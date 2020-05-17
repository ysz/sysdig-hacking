# How to get started hacking sysdig and falco

time took `make -j 16` t3.2xlarge is 20m , z1d.2xlarge is 15m

TODO: create ec2 instance
TODO: add build playbook

```
./bootstrap.sh
# TODO create ec2 instance
./.venv/bin/ansible-playbook --private-key YSZ.pem -i ec2-34-219-255-115.us-west-2.compute.amazonaws.com, --extra-vars "ansible_user=ubuntu" sysdig-playbook.yml
```
