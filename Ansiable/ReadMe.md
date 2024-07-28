This is all the Ansiable scripts I use in our Vast inviroment. This was a must have due to the scale of our inviroment.

Add your Vast API key to playbooks/Install.yaml line 168 where it says "API Key Here"

Host ini is where you will put the IP/Hostnames of the servers that you want to run the playbooks on.
By defult the playbooks are using "*" witch will use any server no matter the group in the ini file you can specify the group if you want.

I use MAAS in my inviorment so to run the scrips with MAAS use.
```ansible-playbook test.yaml -i ~/Ansiable/inventory/hosts.ini -u ubuntu```