Repo: Windows-admin
File: apache2-manage-website.md

1. ⭐ Overview
In this lab, I deployed and configured the Apache2 web server on a Debian-based environment. I replaced the default Apache site with a custom company website, created a dedicated virtual host, and enabled Server‑Side Includes (SSI). This lab simulated real sysadmin responsibilities: managing web content, configuring virtual hosts, enabling modules, and troubleshooting service behavior.

2. 🎯 Objectives
Install Apache2 and verify service operation
Deploy the company website into /var/www/ourcompany
Create and enable a custom virtual host (001-ourcompany.conf)
Disable the default Apache site
Enable Server‑Side Includes (SSI)
Validate that the site loads correctly and SSI works

3. 🛠️ Tools & Commands Used
Linux Commands
ls -l
cat
cp
nano
mkdir
chown
Apache2 Commands
sudo apt install apache2
sudo service apache2 start
sudo service apache2 reload
sudo service apache2 status
sudo a2ensite 001-ourcompany.conf
sudo a2dissite 000-default.conf
sudo a2enmod include

4. 🧩 Steps Completed
A. Install Apache2
Updated package lists
Installed Apache2 and dependencies
Started Apache manually due to lab restrictions
Verified service status
B. Deploy Company Website
Copied site files from /opt/devel/ourcompany
Created /var/www/ourcompany
Set correct ownership for the directory
Verified HTML, CSS, and SSI include files
C. Configure Virtual Host
Created 001-ourcompany.conf in /etc/apache2/sites-available
Set DocumentRoot /var/www/ourcompany
Added <Directory> block with SSI settings
Enabled the new site
Disabled the default site
Reloaded Apache2
D. Enable Server‑Side Includes (SSI)
Enabled the include module
Added:
 Options +Includes
XBitHack on
 inside the <Directory> block
Reloaded Apache2
Verified SSI using <!--#include file="footer.html" -->

5. 🐞 Problems & Fixes
Problem
Fix
Apache2 did not auto-start due to lab policy restrictions
Started manually using sudo service apache2 start
FQDN warning (AH00558) appeared
Identified as harmless; optional fix available but not required
SSI not active by default
Enabled include module and added correct <Directory> configuration


6. 📚 What I Learned
How to deploy and manage Apache2 on Debian
How to configure virtual hosts and replace the default site
How to enable and test SSI
How to troubleshoot Apache2 startup behavior in restricted lab environments
How to structure a web server directory and manage site files

7. 📎 Related Files
/etc/apache2/sites-available/001-ourcompany.conf
/var/www/ourcompany/index.html
/var/www/ourcompany/footer.html
/opt/devel/ourcompany/ (source files provided by the lab)

8. 🔜 Next Steps
Practice enabling SSL and HTTPS
Configure Apache logging and log rotation
Explore reverse proxy configuration
Deploy multiple virtual hosts
Integrate Apache2 with PHP or Python applications

