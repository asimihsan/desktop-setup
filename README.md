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

after you install asdf you'll need ansible installed as well):

```
pip install ansible
asdf reshim python
```

This repo deliberately "vendors" galaxy roles (checks them into the same repo). You can update them by running:

```
ansible-galaxy install -r requirements.yml
```

## Running

Clone then:

```
ansible-playbook -i "localhost," -c local local.yml --ask-become-pass
```

## References

-   https://opensource.com/article/18/3/manage-workstation-ansible
-   https://opensource.com/article/18/3/manage-your-workstation-configuration-ansible-part-2
-   https://opensource.com/article/18/5/manage-your-workstation-ansible-part-3
-   https://stackoverflow.com/questions/22201306/ansible-galaxy-roles-install-in-to-a-specific-directory