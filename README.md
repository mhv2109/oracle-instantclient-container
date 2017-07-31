# oracle-instantclient-container

Add Oracle-instantclient to your [Ansible Container](https://github.com/ansible/ansible-container) project.

Uses alien to convert RPM packages to DEB packages to install with apt on Debian-based images.

Add a variable {{ instantclient_oracle_packages }} with a list of rpm_name, deb_name pairs.

Mount the directory with instanclient installer to /installers/oracle (default).

```
# Set the working directory to your Ansible Container project root
$ cd myproject

# Install the service
$ ansible-container install ansible.oracle-instantclient-container
```