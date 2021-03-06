# AnsibleProject2
WordPress with Ansible

## Architecture Diagram
   - Application (Wordpress)
     Requirements

       LAMP (Linux, Apache, MySQL, PHP) Stack


## Prerequisites:
- AnsibleServer
- LAMP Stack
    - Web-server - Apache, PHP
    - Database - MariaDB

## Usage

## Resources

## Useful Links
  # for php installation >
  # https://www.cyberciti.biz/faq/how-to-install-php-7-2-on-centos-7-rhel-7/  


## Notes
    
    # error 1> if you get the error >  you have to add the metalink 
     # it comes from repository 
    # fatal: [web-server]: FAILED! => {"changed": false, "msg": "Parameter 'baseurl', 'metalink' or 'mirrorlist' is required."}

    # error2> if you get the error  > you have to add description 
    # it comes from repository 
    # fatal: [web-server]: FAILED! => {"changed": false, "msg": "Parameter 'description' is required."}

    # You have to go "yum repos: On CentOS7"
    # Location: ""/etc/yum.repos.d/""  you have to check 
    # ansible -i inventory.yaml web-server -m command -a "php -v" for checking php version using add-hoc command