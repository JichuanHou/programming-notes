## set proxy
[Config ](https://learn.microsoft.com/en-us/windows/wsl/wsl-config#wslconfig) .wslconfig

## ssh from another machine
[Edit](https://gist.github.com/SomajitDey/ec8257ae781234e2a63f3eb731864765) /etc/ssh/sshd_config.
```
Port 2222
AddressFamily any
ListenAddress 0.0.0.0
ListenAddress ::
PasswordAuthentication yes
```
[Add a Hyper-V firewall rule to allow inbound traffic to WSL to the SSH port.](https://github.com/microsoft/WSL/issues/10597#issuecomment-1756461853) `New-NetFirewallHyperVRule -DisplayName "allow WSL ssh" -Direction Inbound -LocalPorts 22 -Action Allow`

Restar ssh as: `sudo service ssh --full-restart`

`ssh localhost -p 2222` should work now.