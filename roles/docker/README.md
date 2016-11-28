#How to use the Docker role

Create a playbook file for docker, for eg. docker.yml in playbook dir.

Given below is sample docker.yml playbook file. Here in this sample, we have specified the docker user called sharad and admin

## playbook/docker.yml
<pre>
---
- name: Install and configure docker
  hosts: docker
  become: yes
  roles:
    - role: docker
      docker_users:
        - sharad
        - admin
</pre>