# Memo VirtualBox
Memo for VirtualBox (Command lines)
* List vms and show infos:
```bash
sudo vboxmanage list -l vms
```
* Delete a vm and the corresponding files / folders:
```bash
sudo vboxmanage unregistervm VM_NAME --delete
```
