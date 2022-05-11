# 1 - Puppet
- nginx
- create configuration files for Nginx to use server names update with puppet
- All dependencies of WordPress
- Install MySQL
- deploy WordPress
- add NTP
- add docker
- add docker-compose
- add python 3.7
- Add unit testing of each component
# 2 - Solution Design
## Scenario: 
```
We have an eCommerce application that has video streaming for products, inventory showcase, Backoffice, front office, website.
The above solution is divided into below services to be run and expected traffic is 2000 concurrent connections we need architecture design along with services and tools with architecture design
```

- 3 stateless java-based Microservices
- 2 python microservices
- 1 PHP Services
- 1 ETL engine
- One back office frontend on ReactJS, one front office frontend on NextJS, and the website is on AngularJS
- Each microservice has its own database.
- Edge Caching is required

# Solution's Acceptance Criteria :
- Design must be self-explanatory.
- Design must have high availability in all possible areas
- Design must have networking components.
- preferred cloud AWS

# 3 - Infrastructure As Code:
- Build distributed infrastructure using Cloudformation/terraform
- Requirements:
- Public-Private subnets in multi-AZ
- create EC2 resources with High availability (Autoscaling Groups)
- Create Database in private subnets
- Ensure EC2 has proper access to DB
- Put load balancer on top of EC2 resources
