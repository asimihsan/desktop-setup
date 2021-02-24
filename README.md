# desktop-setup
Scripts for setting up a Linux/Mac desktop

## Prerequisites - Ubuntu

Install Git and Ansible

```
sudo apt install -y git
sudo apt-get install software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
```

## Running

```
sudo ansible-pull -U https://github.com/asimihsan/desktop-setup.git
```

## References

-   https://opensource.com/article/18/3/manage-workstation-ansible
-   https://opensource.com/article/18/3/manage-your-workstation-configuration-ansible-part-2