# Домашнее задание к занятию "08.04. Работа с Roles"


![img_2.png](img_2.png)

![img_3.png](img_3.png) 

* [Playbook](https://github.com/EvgeniyaAvdeeva/playbook_8.4)
* [clickhouse-role](https://github.com/EvgeniyaAvdeeva/clickhouse-role)
* [vector-role](https://github.com/EvgeniyaAvdeeva/vector-role)
* [lighthouse-role](https://github.com/EvgeniyaAvdeeva/lighthouse-role)


|                           | [vector-role](https://github.com/EvgeniyaAvdeeva/vector-role)            | [lighthouse-role](https://github.com/EvgeniyaAvdeeva/lighthouse-role)                                                                                                                                                       |
|---------------------------|:-------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Role Name                 | Downloads the rpm file and install Vector.                               | Copies Lighthouse from the Git repository and installs                                                                                                                                                                      |
| Preliminary requirements  | Distribution linux: Centos7                                              | Distribution linux: Centos7                                                                                                                                                                                                 |
| Role Variables            | In the file defaults/main.yml:<br/> - vector_version: "0.21.0"           | In the file vars/main.yml:<br/>- lighthouse_vcs: https://github.com/VKCOM/lighthouse.git <br/> - lighthouse_access_log_name: lighthouse_access<br/>- lighthouse_location_dir: ~/home/lighthouse<br/>nginx_user_name: "root" |
| Dependencies              | There are no dependencies                                                | First you need to install epel-release, download nginx and install git                                                                                                                                                      |
| Example Playbook          | - name: Install Vector<br/> hosts: vector<br/> roles:<br/> - vector-role | - name: Install Lighthouse<br/> hosts: lighthouse<br/> roles:<br/> - lighthouse-role                                                                                                                                        |
| License                   | Free                                                                     | Free                                                                                                                                                                                                                        |
| Author Information        | Evgeniya Avdeeva                                                         | Evgeniya Avdeeva                                                                                                                                                                                                            |



  
  
    









---

