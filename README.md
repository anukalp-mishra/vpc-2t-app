<h1>Project Introduction</h1>
<h3>In this project we'll demonstrate how to create a VPC that we can use for servers in a production environment.</h3>
<p>To improve resiliency, we need to deploy the servers in multiple Availablity Zones and here we're going use 2 AZ, by using an Auto Scaling group & an Application Load Balancer (LB).
For additional security, we'll deploy the servers in private subnets. The servers receive request through the LB. The servers can connect to the internet by using a NAT gateway. Tp improve resiliency, we'll deploy the NAT gateway in both Availablity Zones.</p>
