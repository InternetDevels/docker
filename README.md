# Repo with docker images and examples.
## What's inside
- `examples/`
    Folder with examples how we are using official or other existing images if they satisfy our needs.
- `images/`
    Docker images created by our developers for some special tasks.
- `install-docker/`
    [Ansible](https://www.ansible.com/) playbook designed to automate docker installation on any Ubuntu system.
    
    
## List of services we are working on
### For Developers
##### Production ready
- Web (s6, php, nginx/apache, drush, drupal console)
- MariaDB
- Solr
- Redis
- Memcached
- Node.js
- Varnish

##### Local Development only
- Web_local (xdebug, xhprof)
- Adminer
- phpMyAdmin
- MailHog
- Frontend stuff (node+npm+compass)


### For QA
- [Jenkins](images/jenkins)
- [Selenium](examples/selenium-chrome)
