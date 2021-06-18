# Setting Up d.ASH VPN

When setting up VPN for d.ASH, two separate login credentials are required for two seperate VPN connections - one for the robot onboard computer and one for the remote client. This section of the d.ASH SDK documentation provides details about setting up the d.ASH VPN. 

---

### 3.1 ^^Setting Up VPN Onboard Computer^^

To start, you will need to install some packages to configure automatic VPN connection on Ubuntu 18.04 LTS by executing the following command:

``` python3
sudo apt install network-manager-openvpn network-manager-openvpn-gnome openvpn openvpn-systemd-resolved -y
```

This will install an `openvpn` package, which creates a `/etc/openvpn/client/` directory into which you can place the OpenVPN client configuration file. You will need to configure the VPN configuration file - `client.ovpn` which can be found in your vpn folder `/dash_sdk/vpn`. To do so, run the following command:

``` sh
dash-sdk/
└─ vpn/
    └─ client.ovpn
    └─ ca.crt
    └─ <user>.crt
    └─ <user>.key
```
Note that `<user>` in this instance is replaced by your dConstruct admin username. Now, you will need to copy `client.ovpn` and your user certifications - `ca.crt`, `<user>.crt`, `<user>.key` - into the new open-vpn directory. In the `/dash_sdk` directory, execute the following commands:

``` python3
python3.7 configVPN.py
sudo cp client.ovpn /etc/openvpn/client/client.conf 
sudo cp ca.crt <user>.crt <user>.key /etc/openvpn/client
```

For example, if your dConstruct admin username is `user123`, you would replacing `<user>` with `user123`:

``` python3
sudo cp client.ovpn /etc/openvpn/client/client.conf 
sudo cp ca.crt user123.crt user123.key /etc/openvpn/client
```

To check that your files have been copied and renamed correctly, `cd` into the `/etc/openvpn/client` directory and `ls` to see your list of files. You should have `client.conf` and your user certification files, namely `ca.crt .crt .`:

``` python3
cd /etc/openvpn/client
ls
```
``` sh
etc/
└─ openvpn/
    └─ client/
        └─ client.conf
        └─ ca.crt
        └─ <user>.crt
        └─ <user>.key
```

Now, let's test that the VPN service was set up correctly by running the following command:
``` python3
sudo systemctl start openvpn-client@client.service
```

If there is no error print, proceed onto the next step. If you come across a failure, ensure that the path in `client.conf` matches the following format:

```python3
cat \etc\openvpn\client\ca.crt
cert \etc\openvpn\client\<user>.crt
key \etc\openvpn\client\<user>.crt
```

Now, to check your VPN status, enter the following command: 
``` python3 
sudo systemctl status openvpn-client@client.service
```
If successful, you should be able to see the status `Initialization Sequence Completed`. Lastly, enable the VPN onboard your computer by executing the following command: 

``` python3
sudo systemctl enable openvpn-client@client.service
```

---

### 3.2 ^^Setting Up VPN Remote Client^^

Remember to use a separate login credential from the robot onboard computer credentials as at any point in time, there can only be one active user session.

Firstly, download [OpenVPN Connect](https://openvpn.net/client-connect-vpn-for-windows/). Once OpenVPN has been launched, click on the tab - _'Import from File'_ tab and drag-and-drop the `client.ovpn` file located in `\dash-sdk\vpn`. It is important to note that the `client.ovpn` file has to be in the same directory as there certification files, namely `ca.crt .crt .key`:

``` sh
dash-sdk/
└─ vpn/
    └─ client.ovpn
    └─ ca.crt
    └─ user.crt
    └─ user.key
```