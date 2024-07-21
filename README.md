## Apt repository, powered by Ansible
This role provides a means to configure a simple Apt repository for use with Debian-like systems.

It can be installed on either RedHat or Debian and will use Apache as the webserver without authentication.

NOTE: RHEL-like systems require EPEL to be configured

SSL is a mandatory setting, but you can use self-signed certificates if required.

# Usage
* Install the role (either from Galaxy or directly from GitHub)
* Copy the defaults file to your inventory (or wherever you store them) and
  fill in the blanks
* Add the role to your master playbook
* Run Ansible
* ???
* Profit!

# Adding packages
After setting up the repo server you can add packages with the following script:

/usr/local/bin/aptrepo-add [package] [repo_name]
