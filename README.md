---
- hosts: all
  gather_facts: yes
  - name: install httpd
    yum:
      name: httpd
      state: present

