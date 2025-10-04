<p align="center">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/92/Logo_Proxmox.svg/1200px-Logo_Proxmox.svg.png" width="600">
</p>

## About

Instructions on how to disable paid repositories and notifications about not subscriptions

## My Links

- [DS: RedstoneLink](https://discord.gg/BE8fEbJ9HJ)
- [Site: RedstoneLink](https://RedstoneLink.ru)
- [TG: RedstoneLink](https://t.me/redstonelink)

## Developers

- GitHub - [MASHINIST [YT]](https://github.com/MASHINISTPROJECT)
- Youtube - [MASHINIST [YT]](https://www.youtube.com/@MASHINIST_8888)

## Steps:
- disabling paid repositories:
- `go to the proxmox control panel, select your node, and go to the updates section. Below that, you will find the Repositories section.
  disable all paid repositories and add a non-subscription repository
  Next, go to the Updates section and click the Refresh button. Wait for all the repositories to be found and the message TASK: OK to appear.
  the last step is to click on the upgrade button to update the system and wait for the end. Congratulations, you have successfully updated Proxmox!`
- disabling the unsubscribe sign:
- `When you select a node, you will see a shell button. Click on it and proceed to the next steps.
  write a command to navigate to the directory: cd /usr/share/javascript/proxmox-widget-toolkit
  write a command to edit the file: nano proxmoxlib.js
  press the ctrl + w keyboard shortcuts and paste: No valid
  change Ext.Msg.show({ to void({
  save the file: ctrl + x, next Y, next Enter
  Restart the service with the command: systemctl restart pveproxy
  Done! Log out of your account in the proxmox panel and reload the page with ctrl + f5, then log in again and you won't see this message anymore!`
