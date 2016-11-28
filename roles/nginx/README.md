#How to use Nginx role

Create a playbook file for Nginx, for eg. nginx.yml in playbook dir.

Given below is sample nginx.yml playbook file. 

## playbook/nginx.yml
<pre>
---
- name: Install and configure nginx
  hosts: nginx
  become: yes
  roles:
    - { role: nginx }
</pre>