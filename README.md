# Memo VirtualBox
Memo for VirtualBox (Command lines)
* Import an OVA file with specific mount folders (ex hipchat):
```bash
sudo VBoxManage import -vsys 0 --unit 12 --disk /home/xxx/vbox_hipchat_mount/chat_history.vmdk --unit 13 --disk /home/xxx/vbox_hipchat_mount/file_store.vmdk --unit 14 --disk /home/xxx/vbox_hipchat_mount/system.vmdk --ostype Ubuntu_64 -eula accept --vmname hipchat /home/xxx/hipchat/HipChat.ova
```
* List vms and show infos:
```bash
sudo vboxmanage list -l vms
```
* List running vms:
```bash
sudo VBoxManage list runningvms
```
* Delete a vm and the corresponding files / folders:
```bash
sudo vboxmanage unregistervm VM_NAME --delete
```
* List system properties:
```bash
sudo VBoxManage list -l systemproperties
```
* Change default machine folder:
```bash
sudo VBoxManage setproperty machinefolder /home/xxx/vbox_default_folder
```
