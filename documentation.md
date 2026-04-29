## Setup Web Server Using Apache and AWS EC2 Instance

This project is to create a secure and scalable web server on AWS EC2 configuring Apache2 as the web server software and hosting a simple, professional static landing page for Elite Corporation.

**Steps**

1. Go to EC2 on AWS Console, create and launch an instance. 

    a. Set name for your instance 

    ![1](images/apache%202.png)

    b. Choose **Ubuntu** as AMI under Quick Start

    ![1](images/apache%203.png)

    c. Create new key pair or use an exising one

    ![1](images/apache%204.png)

    d. Enable traffic from the internet by clicking the checkboxes, then click **"Launch instance"**. After instance is launched, Connect to instance.

    ![1](images/apache%205.png)

    e. On the *Connect* page, click *Connect using Public IP* to Connect to instance and the Ubuntu terminal comes up.

    ![1](images/apache%207.png)

2. After the terminal comes up, run the following commands to install and setup the apache server:

    *sudo apt update*   -- To setup the Apt package manager used to install packages on Ubuntu

    *sudo apt install apache2*  -- To install the Apache server

    *sudo systemctl start apache2*  -- To start the Apache server

    *sudo systemctl enable apache2* -- To enable boot time so the Apache server runs automatically

    *sudo systemctl status apache2* -- To confirm boot time is enabled

    ![1](images/apache%208.png)

    ![1](images/apache%209.png)

    ![1](images/apache%2010.png)

3. Copy the Public IP address from your instance and paste on your browser. Upon launch of Apache2 Default page, it indicates our instance is running properly.

    ![1](images/apache%2011.png)

4. To host our website on the Apache server, we replace the index file containing the Apache default page with our html file for our website.

    ![1](images/apache%2012.png)

    ![1](images/apache%2013.png)

5. Reload the web page with the IP address to ensure the web page has been hosted successfully.

    ![1](images/apache%2014.png)

    ![1](images/apache%2015.png)

6. Terminate instance on EC2 at the end of the task.

