---
- hosts: all
  gather_facts: yes
  # To install package
  - name: install httpd
    yum:
      name: httpd
      state: present
    service:
      name: httpd
      state: restarted
