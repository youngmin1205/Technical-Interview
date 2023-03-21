# Solutions Architect Interview Questions AWS by Cloud With Raj (Youtube)

## Q. How can you make your application scalable for a big traffic day?
<details>
<summary>
Average Answer</summary>
<div markdown="1">
 <img width="333" alt="img3" src="https://user-images.githubusercontent.com/35551015/226612776-f9c527a8-66ff-4827-8695-5d82721a43e2.png"> <br>
Put the VMs or EC2 in auto scaling group and use load balancer
</div>
</details>

<details>
<summary>
Good Answer</summary>
<div markdown="1">
<img width="487" alt="img2" src="https://user-images.githubusercontent.com/35551015/226612899-769cdd1d-bf6e-4c99-8b0b-21a4f7a6e566.png"> <br>
For a big traffic day like Black Friday or Christmas, If I let load balancer to scale up naturally, it may not able to keep up with raised traffic.<br>
To avoid that, will pre-warn my load balancer before the a big traffic event. Similarly, will use “Scheduled Scaling” for my auto scaling group. So all that necessary EC2s are up and running with application on it. So when traffic increases, they are ready to go.<br>

In case load balancer needs to be scaled up naturally, will make sure Application Machine Image (AMI) is as light-weight as possible. The more unnecessary libraries you put into AMI, the longer it will take for EC2 to spin up.<br>

If my application is connected to database, I will utilize the database proxy(e.g. RDS proxy), in case of high traffic, sometimes application will make rapid new connection to database and when the program stop querying the database for the particular instance, the connection will stay open. So when another traffic invocation comes, instead of reusing that lingering orphan connection, it will create **another new connection**. So this results in lots of orphan database connections taking up precious compute from your database. **Using RDS proxy will eliminate that. RDS proxy will maintain the database connection full, it will reuse the orphan database connections, it will terminate as needed.** <br>

And on top of this, I will run IEM to ensure it can handle high traffic. IEM is a event that AWS runs before the big traffic day so it will scale up the load balancer, EC2, and then it will pass a high traffic to ensure that the application can handle it.<br>

Beyond this, you can also talk about breaking the app into microservices (talks about advantages of microservices). One specific API might need to scale up way more than another microservice in same application. Using microservice, you can utilize that individual scaling of each APIs.<br>

Just migrate my application to Kubernetes or Serverless then it will handle the big traffic days which is **not true,** because Kubernetes and Serverless, they all have their scaling limits.
</div>
</details>


## Q. How did you do DR for your cloud application??
<details>
<summary>
Average Answer</summary>
<div markdown="1">
Replicate to another region
</div>
</details>

<details>
<summary>
Good Answer</summary>
<div markdown="1">
There are different options to choose from depending on RTO and RPO.<br>
<img width="454" alt="img5" src="https://user-images.githubusercontent.com/35551015/226614713-87cab72d-6f7e-4e0b-9594-63fe3c1cd56d.png"> <br>
Tip: Have one option ready in detail with example.<br>
<img width="459" alt="img6" src="https://user-images.githubusercontent.com/35551015/226614830-7f45b880-11f3-41bd-b636-768da4673d72.png">
<br>
I would have two load balancers in two different regions. Those are fronting front end and maybe application server and Route53 can send traffic to appropriate region based on the latency, so even if one region goes down, Route53 will automatically send all the traffic to the other region.<br>

For the database, if I use dynamoDB, I will use dynamoDB global tables which will automatically replicate along with continuous backup.
</div>
</details>


## Q. How do you secure your application on the cloud?
<details>
<summary>
Average Answer</summary>
<div markdown="1">
Use KMS, IAM and firewalls for security
</div>
</details>

<details>
<summary>
Good Answer</summary>
<div markdown="1">
Tip: <br>
 - Explain what they do rather than just saying service names <br>
 - Take one app (such as three tier app with EC2, or microservice running on Kubernetes, or Serverless and explain in detail) <br>

Assuming my application is running in a serverless manner, so all the APIs are hosted in Amazon API Gateway and all the API back end are handled by Lambda and then that Lambda is going to different DBs.<br>

Three different colored arrows = there are three microservices running <br>

On user side, will implement authentication, secure data transit using SSL/TLS. On API Gateway, will implement authentication and authorization layer. The security of data at rest, you encrypt the data at rest using KMS. <br>

**Tip: The most important part is “Security of the application” part because this is where you probably get the most of the questions.** <br>
e.g. Security of the application - Kubernetes <br>
In Kubernetes, generally you have your application container image running within a pod and that pod is running in EC2. <br>

</div>
</details>


## Q. Describe an architecture you designed
<details>
<summary>
Good Answer</summary>
<div markdown="1">
Tips: Always better to explain I used microservice you designed, even if it is small.<br>
  e.g. microservice design with third party API Gateway with Lambda <br>
 <img width="460" alt="img1" src="https://user-images.githubusercontent.com/35551015/226550195-2a578675-d1dd-407a-b888-afbbabe588c6.png">
</div>
</details>



## Q. Biggest challenge faces on cloud
<details>
<summary>
Average Answer</summary>
<div markdown="1">
There are so many services, so it’s hard to determine when to use for what.
</div>
</details>

<details>
<summary>
Good Answer</summary>
<div markdown="1">
e.g. Auto scaling - thought using a regular auto scaling group would take care of high burst, high scaling criteria but it did not, so then had to do all the additional things.

e.g. Cost optimize the application - tried to design a kubernetes application but there is no restrictions on how big the parts could be, how big the nodes could be. So the application is just spinning up stuff and incurring a lots of bill, even if we are not using whatever we are spinning. To fix it, Amazon CloudWatch Insights and AWS Compute Optimizer identify whether aws resources are optimal and offer recommendations to improve cost and performance 
(Other option: the spot instances, AWS Cost Explorer for research purpose, third party(Kubecost, CloudHealth))
</div>
</details>


## Q. How do you pick one service vs another as a solutions architect?
<details>
<summary>
Average Answer</summary>
<div markdown="1">

</div>
</details>

<details>
<summary>
Good Answer</summary>
<div markdown="1">
</div>
</details>


## Q. What is the difference between SQL and NoSQL?
<details>
<summary>
Average Answer</summary>
<div markdown="1">

</div>
</details>

<details>
<summary>
Good Answer</summary>
<div markdown="1">
</div>
</details>

## Q. What is the Cloud Computing?
<details>
<summary>
Average Answer</summary>
<div markdown="1">

</div>
</details>

<details>
<summary>
Good Answer</summary>
<div markdown="1">
</div>
</details>
