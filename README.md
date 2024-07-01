# Terraform-VPC-project
![vpc](https://github.com/TintinSDev/Terraform-VPC-project/assets/69876670/02056eba-160d-450d-98aa-89a0ad9ba3dd)

### Link to Terraform AWS documentation page 
🌐 https://registry.terraform.io/providers/hashicorp/aws/latest/docs

# Terraform Project: VPC Setup

## Steps
** create a main.tf and provider.tf file
1. **Create VPC (Virtual Private Cloud)**
   - Define and initialize your VPC.
   - https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc
   
2. **Create Two Subnets (Public & Private)**
   - Define both public and private subnets within the VPC.

3. **Create Security Group**
   - Set up security groups to manage inbound and outbound traffic rules.
   - https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/security_group

4. **Create Internet Gateway (IGW)**
   - Attach an Internet Gateway to the VPC for external access.
   - https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/internet_gateway

5. **Route Table for Public Subnet**
   - Define a route table and associate it with the public subnet.

6. **Route Table Association**
   - Associate the route table with the public subnet.
   - https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table
   - https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route_table_association

7. **Create Instance (Web Server) and Connection**
   - Launch a web server instance and configure it for connectivity.

8. **Create Elastic IP and Associate with Web Server**
   - Allocate an Elastic IP and associate it with the web server instance.

9. **Create Instance for DB Server**
   - Launch a database server instance within the private subnet.

10. **Create NAT Gateway**
    - Set up a NAT Gateway for the private subnet to access the internet.

11. **Create Route Table for NAT Gateway and Associate**
    - Define and associate a route table for the NAT Gateway.
    - https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/route
    - https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/nat_gateway

