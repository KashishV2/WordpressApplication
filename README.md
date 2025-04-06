
# Deploy a Highly Available WordPress Application

Welcome to my ✨**WordPress on AWS EC2**✨ project with a fully customized frontend using **HTML, CSS, and JavaScript** inside a custom theme.

*Create a highly available (HA), scalable and fault-tolerant deployment of the WordPress application. You will deploy the WordPress application in such a way that the application server, load balancer and database will scale independently of one another. You will also deploy the application's components like the webserver and database into two availability zones to distribute it and guard against failure of the anyone availability zone. The WordPress application will be deployed in a stateless fashion so that we can add or remove web application servers in response to the requests flowing into the system. Finally, we create a CloudFront distribution as CDN and change the configuration of WordPress.

## What I Built

- ✅ WordPress installed on an EC2 instance (Amazon Linux)
- ✅ MariaDB for database setup
- ✅ Custom theme created from scratch (`awesome-theme`)
- ✅ Connected to S3 and CloudFront for speed + scalability
- ✅ Secure config with `.htaccess`, CloudFront, and DB credentials
- ✅ Responsive frontend with HTML/CSS + JavaScript interactions
- ✅ Ready for deployment with GitHub versioning


---
## Project Structure

awesome-theme/
│
├── style.css          # Theme metadata + custom styles
├── index.php          # Main theme template with custom HTML
├── functions.php      # Theme setup + enqueue scripts
└── assets/
    ├── banner.jpg     # Custom banner image
    ├── script.js      # Custom JavaScript


## Deploy Wordpress

1. EC2 Setup--
sudo yum update -y
sudo yum install -y httpd mariadb-server php php-mysqlnd php-dom php-gd

2. Wordpress Installation
cd /var/www/html
wget https://wordpress.org/latest.tar.gz, 
tar -xzf latest.tar.gz
sudo mv wordpress/* .

4. Create Database User in MariaDB
CREATE USER 'wordpress-user'@'localhost' IDENTIFIED BY 'yourpassword';
GRANT ALL PRIVILEGES ON *.* TO 'wordpress-user'@'localhost';
FLUSH PRIVILEGES;

5. Set Up Custom Theme
cd /var/www/html/wp-content/themes
sudo mkdir awesome-theme
cd awesome-theme
create style.css, index.php, and functions.php

## Features

🎨 1. Custom WordPress Theme
Built entirely from scratch using HTML, CSS, and JavaScript.

Fully functional and integrated with WordPress CMS.

📁 2. Organized Theme Structure
* Clean Folder Hierarchy

🌄 3. Hero Banner
Displays a custom banner image from the assets/ folder.

Perfect for portfolio, landing pages, or product showcases.

🧠 4. Dynamic JavaScript Functionality
Basic interactivity using custom JavaScript:

Page load alerts

DOM manipulation possibilities

Extendable for more UI magic (sliders, animations, toggles, etc.)

🎨 5. Responsive & Custom Styling
Styled with modern CSS for clean visuals.

Can be extended using Flexbox/Grid for responsiveness.

🔧 6. Enqueued Assets
JS & CSS files are enqueued properly using functions.php — best practice for WordPress theme devs.

⚙️ 7. Cloud Integration Ready
Runs on AWS EC2 + WordPress setup.

Can be accessed via CloudFront domain for speed & CDN support.

💻 8. Developer-Friendly
Easy to understand code structure.

Can be uploaded to GitHub and shared with the dev community.

## 🧠 Why This Project?

I wanted to learn how to host a full WordPress site on AWS using EC2, integrate S3/CloudFront, and also design my own frontend theme using core web technologies.

## Screenshots
 # Wordpress Dashboard
![{66743EE6-78F8-4E20-BC98-F9F32F3222AF}](https://github.com/user-attachments/assets/2ff203ea-c656-4f35-8818-d1ca8f48ba72)
 # CloudFront(CDN)
![{CD608F00-DEA4-425D-9C4D-C3AE9FA510EA}](https://github.com/user-attachments/assets/8a15e6af-2777-48a7-b404-2c39f3ec5c61)
# Custom Theme
![{9B8443C5-188A-40C0-BCAC-D2AA407C51DC}](https://github.com/user-attachments/assets/4c10f120-847c-476d-8743-021033afbd4f)
# PHP
![{2D299B9A-329E-4BAE-B777-1E3901A28519}](https://github.com/user-attachments/assets/ac8ac9b5-0fd2-4f9c-951a-12e3996fbcca)

## 🚀 About Me
I'm a full stack developer...

## 🔗 Links
http://www.linkedin.com/in/kashish-varshney-166333273










