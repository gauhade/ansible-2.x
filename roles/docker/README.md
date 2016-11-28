<title>How to use the Docker role</title>

Create a playbook file for docker, for eg. docker.yml in playbook dir.

Given below is sample docker.yml playbook file. Here in this sample, we have specified the docker user called sharad and admin

<pre>
---
- name: Install and configure nginx
  hosts: docker
  become: yes
  roles:
    - role: docker
      docker_users:
        - sharad
        - admin
</pre>