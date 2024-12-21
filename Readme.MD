## Alt School Second Semester Project Documentation

## Question

“Imagine you are part of a startup team tasked with creating a prototype for a web application. Your first step is to provision a server and set up a simple landing page to demonstrate your team’s capabilities to potential investors. Your task is as follows:”

### Provisioning the Server:

* Use any virtualization or cloud platform (AWS.) to set up a Linux server.
* Install a Linux distribution of your choice (e.g., Ubuntu).

### Web Server Setup:
* Install a web server (e.g., Apache, Nginx) to serve web content.

### HTML Page Deployment:
- Create a simple HTML page with the following  information: 

  - Your name.
  - A project title: “Welcome to [Your Name] Landing Page.”
  - A brief description of your project.
  - Your full bio with every interesting information about you
  - Deploy the HTML page on the server.

### Networking:

- Configure the server to allow HTTP traffic (port 80).
Provide the public IP address (or URL if using DNS) so your page can be accessed from any browser.

### Deliverables:
- The public IP address or URL of your web page.
- A screenshot showing your HTML page in a browser.
- Write clear, step-by-step documentation of how you provisioned the server, installed the web server, deployed the HTML page, and configured networking.

### Bonus Tasks (Optional for Extra Credit):
- Configure HTTPS for your web server using a free SSL certificate (e.g., Let’s Encrypt).


### Provisioning the Server:

* Use any virtualization or cloud platform (AWS.) to set up a Linux server.

I will be using AWS cloud to provision my server to setup my webpage on the cloud:

- Login to my AWS console to configure and create ubuntu server as required. 

![AWS console](<images/AWS Console.png>)


* Install a Linux distribution of your choice (e.g., Ubuntu).

I would be provisioning and configuring Ubuntu server using AWS intance. 
Ubuntu server succesfully provisioned with public, private IP and DNS. 

![ubuntu server](<images/ubuntu server provionsed.png>)

### Web Server Setup:
* Install a web server (e.g., Apache, Nginx) to serve web content.

I would be connecting to the Ubuntu server using termius to install and configure Apache web server to serve my webpage content. 

![connected](images/Connected.png)

I would be runing the following commands to intall and configure my Apache server. 

I first change directory to root directory with the command below:

Command: sudo su -

![alt text](images/cdroot.png)

I update the server with the command below to install all the neccessary update to install my Apache and web page using the command below:

Command: apt update -y

![Update](images/installupdate.png)

Update completed:

![update completed](images/updatecompleted.png)

I would be installing Apache with the command below:

apt install -y apache2

![install apache](images/installApache.png)

Apache installation completed:

![apache completed](images/ApacheCompleted.png)

Check System status witht he following command to be sure the system is active:

systemctl status apache2

![systemstatus](images/systemstatus.png)

Create project directory and cd to the project director. 

![projectfolder](images/createfolderandcd.png)


### HTML Page Deployment:
- Create a simple HTML page with the following  information: 

  - Your name.
  - A project title: “Welcome to [Your Name] Landing Page.”
  - A brief description of your project.
  - Your full bio with every interesting information about you
  - Deploy the HTML page on the server.


