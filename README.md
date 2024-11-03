<h1>Project Introduction</h1>
<h3>In this project we'll create a VPC that we can use for servers in a production environment.</h3>
<p>To improve resiliency, we need to deploy the servers in multiple Availablity Zones and here we're going use 2 AZ, by using an Auto Scaling group & an Application Load Balancer (LB).
For additional security, we'll deploy the servers in private subnets. The servers receive request through the LB. The servers can connect to the internet by using a NAT gateway. Tp improve resiliency, we'll deploy the NAT gateway in both Availablity Zones.</p>
<h3>Overview</h3>
<ul>The VPC has public subnets & private subnets in two Availablity Zones.</ul>
<ul>Each public subnet contains a NAT ggateway & a load balancer node.</ul>
<ul>The servers run in the private subnets and are launched & terminated by using an Auto Scaling group, and receive traffic from the load balancer.</ul>
<ul>The servers can connect to the internet by using the NAT gateway.</ul>
