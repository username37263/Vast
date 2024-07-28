This is all the Ansible scripts I use in our Vast environment. This was a must-have due to the scale of our environment.

Add your Vast API key to `playbooks/Install.yaml` line 168 where it says `"API Key Here"`

`hosts.ini` is where you will put the IP/Hostnames of the servers that you want to run the playbooks on. By default, the playbooks are using `"*"` which will use any server no matter the group in the ini file. You can specify the group if you want.

I use MAAS in my environment, so to run the scripts with MAAS, use:

```sh
ansible-playbook test.yaml -i ~/Ansible/inventory/hosts.ini -u ubuntu
