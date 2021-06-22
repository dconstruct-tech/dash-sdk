# d.ASH Service Configuration

This section of the d.ASH SDK documentation provides details about the configuration file for the rest server - `rest_config.json` - found in the folder `\dash-sdk\configs`. Information in this section includes variable and definitions to configure the d.ASH service.

### 1.1 ^^Config File^^

``` python
{
    "port" : 3000,
    "certFilename" : "./cert.pem",
    "keyFilename" : "./key.pem",
    "dhParamsFilename" : "",
    "robotRegisterNativeCert" : true,
    "activeIPIdx" : 1, 
    "preferredIP" : "10.8.0.5", 
    "runCmds" : {
        "py_server" : {
            "cmdStr" : "python ./spot_server.py ./configs/robot_deploy_config.json <!TOKEN!>",
            "cmdPath" : "C:/Users/dc/Documents/Projects/dc/dash_code/py_server"
        }
    }
}
```

### 1.2 ^^Definitions^^

#### 1.2.1 Main

- **`port`**: Fixed port number.
- **`certFilename`**: Fixed certification filename.
- **`keyFilename`**: Fixed certification key filename.
- **`dhParamsFilename`**: Fixed parameter filename.
- **`robotRegisterNativeCert`**:  If you registed with register_bot_native, the data will be encrypted. Always set this variable to true.
- **`activeIPIdx`**: Selects the IP address you will send to the backend cloud service for robot discovery. This is an integer index ( from 0 to N ), based on the IP addresses available on your system. When the rest service starts up, you should see a list. Set the value to the appropriate index you want. This index will map the the IP which the clients will try to connect to
- **`preferredIP`**: Selects your preferred IP from the list of IPs. Specify the IP as a string in this case.

---

#### 1.2.2 d.ASH Server Commands

- **`cmdStr`** : Sets command to run d.ASH server.
- **`cmdPath`** : Sets command path.
