# ansible-role-fail2ban-firewalld
Ansible role to install fail2ban with firewalld

[![Build Status](https://travis-ci.org/HauptJ/ansible-role-fail2ban-firewalld.svg?branch=master)](https://travis-ci.org/HauptJ/ansible-role-fail2ban-firewalld)

## Installation
1. Fork this repository
2. git submodule add <git host> roles/ansible-role-fail2ban-firewalld
    - [submodule reference](https://chrisjean.com/git-submodules-adding-using-removing-and-updating/)

**Ansible Galaxy:** [HauptJ.ansible-role-fail2ban-firewalld](https://galaxy.ansible.com/HauptJ/ansible-role-fail2ban-firewalld/)


## Variables

### Fail2ban Firewalld

| Name 						                  | Default 							                    | Description 										        |
|-----------------------------------|-------------------------------------------|-----------------------------------------|
| f2b_whitelist_ip                  | 8.8.8.8                                   | IP to whitelist                         |
| f2b_destmail                      | bob@example.com                           | Email to send reports to                |
| f2b_sender                        | alice@example.com                         | Email to send reports from              |
| cf_email                          | alice@srv.example.com                     | CloudFlare account Email                |
| cf_key                            | key                                       | CloudFlare account API key              |
| f2b_bantime                       | 3600                                      | IP ban duration in sec                  |
| f2b_findtime                      | 600                                       | time period to count retries in sec     |
| f2b_maxretry                      | 5                                         | nbr of failed attempts in f2b_findtime before ban |
