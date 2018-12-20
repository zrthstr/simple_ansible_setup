
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

### keep changes local

ignore changes to previously added file
```
git update-index --assume-unchanged [<file> ...]
```
revert
```
git update-index --no-assume-unchanged [<file> ...]
```
