# Restaurant Website

This project serves as a website for your first AWS Laboratory. Your task is to launch it on AWS EC2.

## Steps to Launch the Website on AWS EC2

### 1. Create a VPC with Two Availability Zones

1. Log in to the AWS Management Console.
2. Navigate to the VPC Dashboard.
3. Click on "Create VPC".
4. Choose "VPC with Public and Private Subnets" and click "Select".
5. Configure the VPC settings:
   - Name tag: `MyFirstVPC`
   - IPv4 CIDR block: `10.0.0.0/18`
   - IPv6 CIDR block: No IPv6 CIDR Block
   - Tenancy: Default
6. Configure the Subnets:
   - Public Subnet 1: `10.0.1.0/24` (Availability Zone 1)
   - Private Subnet 1: `10.0.2.0/24` (Availability Zone 1)
   - Public Subnet 2: `10.0.3.0/24` (Availability Zone 2)
   - Private Subnet 2: `10.0.4.0/24` (Availability Zone 2)
7. Click "Create VPC".

### 2. Launch an EC2 Instance

1. Navigate to the EC2 Dashboard.
2. Click on "Launch Instance".
3. Choose an Amazon Machine Image (AMI), such as Amazon Linux 2 AMI.
4. Choose an Instance Type, such as `t2.micro`.
5. Configure Instance Details:
   - Network: Select the VPC you created (`MyFirstVPC`).
   - Subnet: Select the second public subnets.
   - Auto-assign Public IP: Enable
6. Add Storage (use default settings).
7. Add Tags (optional).
8. Add Security Group.
9. Review and Launch the instance.
10. Select or create a key pair to access the instance and click "Launch Instances".

### 3. Deploy the Website

1. Connect to your EC2 instance:
2. Install a web server (e.g., Apache):
3. Upload your website files to the EC2 instance:

### 4. Access the Website

Open a web browser and navigate to the public IP address of your EC2 instance. You should see your restaurant website.

## Project Structure

```
about.html
booking.html
bootstrap-restaurant-template.jpg
contact.html
index.html
LICENSE.txt
menu.html
READ-ME.txt
service.html
team.html
testimonial.html
css/
    bootstrap.min.css
    style.css
img/
    about-1.jpg
    about-2.jpg
    about-3.jpg
    about-4.jpg
    bg-hero.jpg
    hero.png
    menu-1.jpg
    menu-2.jpg
    menu-3.jpg
    menu-4.jpg
    menu-5.jpg
    menu-6.jpg
    menu-7.jpg
    menu-8.jpg
    team-1.jpg
    team-2.jpg
    team-3.jpg
    team-4.jpg
    testimonial-1.jpg
    testimonial-2.jpg
    testimonial-3.jpg
    ...
js/
    main.js
lib/
scss/
```

## License

This project is licensed under the MIT License. See the [LICENSE.txt](LICENSE.txt) file for details.

## Contact

For any inquiries, please contact [your-email@example.com](mailto:your-email@example.com).