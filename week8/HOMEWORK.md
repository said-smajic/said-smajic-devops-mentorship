What is done in this task:
- Created AMI image
- Created Load Balancer
- Edited Security Groups so we can access our web app only through LB
- Created Launch Template with AMI image mentioned before
- Created Auto Scaling group with specifications:
  - 2 desired instances
  - 2 min, 4 max instances
  - Dynamic auto scaling if average CPU Utilization > 18%

**Link to the app: http://alb-web-server-527642205.us-east-1.elb.amazonaws.com/**

Dijagram:
<img src="Images/338892347_1940030742996031_4793954539163219917_n.jpg">
Nakon kreiranja ASG:
![](Images/Screenshot 2023-04-15 at 13.25.37.png)
Nakon CPU Stress testa:
![](Images/Screenshot 2023-04-15 at 12.40.21.png)![](Images/Screenshot 2023-04-15 at 12.42.05.png)