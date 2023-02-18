# Ansible Deployment of Laravel with Dependencies

This repository provides an Ansible playbook for deploying a Laravel application with all necessary dependencies.

## Prerequisites:
Before you begin, ensure that you have the following prerequisites:

- A server with Ubuntu 18.04 or higher installed
- Ansible 2.9 or higher installed on your local machine
- SSH access to the server as a user with sudo privileges
- A Laravel application codebase with a composer.json file

## Getting Started
To get started, follow these steps:

1. Clone this repository onto your local machine:




       git clone https://github.com/your-username/ansible-deployment-laravel.git
       
2. Edit the `hosts` file in the root directory to include the IP address or hostname of your server:




       
        [laravel]
        your-server-ip-address-or-hostname
        
        
3. Edit the `vars/main.yml` file to include your application-specific variables, such as the application name, database credentials, and environment variables.





        ansible-playbook -i hosts playbook.yml

4.  This will run the Ansible playbook, which will install all necessary dependencies, configure the server, and deploy your Laravel application.



## What's Included

The playbook includes the following tasks:

- Update the server packages and install necessary dependencies
- Install PHP, PHP extensions, and Composer
- Configure the server environment
- Create a new user for the application
- Create a new MySQL database and user for the application
- Deploy the Laravel application codebase
- Configure the application environment variables
  
  
## Customization
The playbook is designed to be easily customized to suit your specific needs. You can modify the variables in the vars/main.yml file to customize the playbook for your application. Additionally, you can modify the tasks in the tasks directory to add or remove functionality.
   


                     
                     
