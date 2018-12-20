
## Usage

* edit `hosts`
* edit `playbooks/main.yml`
* symlink roles as needed.
```
# example
% cd roles
% ln -s ../../arch_basic_server/
```
* run ansible 'first run' to install python if not found
```
% ansible-playbook playbooks/first.yml -e "ansible_ssh_user=root"
```
* run ansible plabook as needed
```
% ansible-playbook playbooks/main.yml
```
