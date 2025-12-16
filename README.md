**# Домашнее задание к занятию "`8-03`" - `Trunova Vika`**

<ins>## Задание 1 </ins>

#apt update
#apt install postgresql
#wget https://repo.zabbix.com/zabbix/6.0/debian/pool/main/z/zabbix-release/zabbix-release_latest_6.0+debian11_all.deb
#dpkg -i zabbix-release_latest_6.0+debian11_all.deb
#ls -la /etc/apt/sources.list.d/  проверка наличия файлов - есть
#apt update   
#apt install zabbix-server-pgsql zabbix-frontend-php php7.4-pgsql zabbix-apache-conf zabbix-sql-scripts
#systemctl status zabbix-server.service проверка статуса - inactive
#su - postgres -c 'psql --command "CREATE USER zabbix WITH PASSWORD
'\'123456789\'';"'
#su - postgres -c 'psql --command "CREATE DATABASE zabbix OWNER zabbix;"'
#zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql Zabbix
#sed -i 's/# DBPassword=/DBPassword=123456789/g' /etc/zabbix/zabbix_server.conf
#systemctl restart zabbix-server apache2
#systemctl enable zabbix-server apache2
#systemctl status zabbix-server.service статус active(running)
#ip a  
http://158.160.55.249/zabbix


![Скриншот 1](https://github.com/vikawhite/8-03-hw/blob/main/runner/1.png)



---

<ins>## Задание 2 </ins>

#apt install zabbix-agent
#systemctl status zabbix-agent.service статус active(running)
#find / -name zabbix_agentd.conf 
#vim /etc/abbi/zabbix_agentd.conf
#systemctl restart zabbix-agent.service
#systemctl status zabbix-agent.service  статус active(running)
#добавить 2вм windows Server=x.x.x.x
#vim /etc/abbi/zabbix_agentd.conf
#systemctl restart zabbix-agent.service
#systemctl status zabbix-agent.service  статус active(running)

![Скриншот 1](https://github.com/vikawhite/8-03-hw/blob/main/01.png)
![Скриншот 2](https://github.com/vikawhite/8-03-hw/blob/main/3.png)
![Скриншот 3](https://github.com/vikawhite/8-03-hw/blob/main/2.png)


---


