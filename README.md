# ansible0
- Requires Vagrant and Virtualbox
- 'log1' listens, receives, and stores logs from the workers.
- The workers should forward all logs to ‘log1'

```
$ vagrant up
$ ansible -m ping -i hosts -u vagrant all
$ ansible-playbook -v -i hosts main.yaml
