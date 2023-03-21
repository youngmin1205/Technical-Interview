# Solutions Architect Interview Questions AWS by Cloud With Raj (Youtube)

## Q. How can you make your application scalable for a big traffic day?
<details>
<summary>
Average Answer</summary>
<div markdown="1">
Put the VMs or EC2 in auto scaling group and use load balancer
</div>
</details>

<details>
<summary>
Good Answer</summary>
<div markdown="1">
</div>
</details>


## Q. How did you do DR for your cloud application??
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
</div>
</details>


## Q. Describe an architecture you designed
<details>
<summary>
Good Answer</summary>
<div markdown="1">
Tips:
 - Always better to explain I used microservice you designed, even if it is small.<br>
  e.g. microservice design with third party API Gateway with Lambda
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