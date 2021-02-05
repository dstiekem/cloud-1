# cloud-1
## "In this project, you will discover the very bases of the "cloud", what auto-scalingg,load-balancing, CDN... mean"
For this project I used three of Amazon's web services to host a wordpress site on the "cloud".

http://thisisdom-env.eba-39iu8itx.us-east-1.elasticbeanstalk.com/

Amazon offers Elastic Cloud Computing for for web based applications that vary in resource focus (cpu, gpu and ram). 
They also have a nifty manager called Elastic Beanstalk (to reach the cloud get-it) which handles capacity provisioning, autoscaling, load balancing and application health monitoring.
I will also use their RDS Database to store and retrieve information for my website.

## cost
I'm using an educate account which gives me some credits to play around with. If I only provision what I need I use very little andwont be charged too much for my environments.

## security
For each tier (Elastic load balancer, Elastic cloud computing and RDS Database) I will need to specify rules for the inbound traffic of the security groups.


## Instance
Elastic Beanstalk handles autoscaling when an instance is terminated or unhealthy. Depending on what I specified as the minimum number of instances, It'll make sure to scale up to that.

## Stress test
I'll be using https://app.k6.io

## CDN
Content Delivery Network will be handled by a third-party plugin to wordpress called Shift8.

