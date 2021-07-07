# d.ASH Service Configuration

This section of the d.ASH SDK documentation provides details about the configuration file for the rest server - `dash_service_config.json` - found in the folder `\dash-sdk\configs`. Information in this section includes variable and definitions to configure the d.ASH service.

### 1.1 ^^Config File^^

``` python
{
    "port" : 3000,
    "cert_filename" : "./cert.pem",
    "key_filename" : "./key.pem",
    "dh_params_filename" : "",
    "robot_register_native_cert" : true,
    "active_IP_idx" : 1, 
    "preferred_IP" : "10.8.0.5", 
    "run_cmds" : {
        "py_server" : {
            "cmd_str" : "python ./spot_server.py ./configs/dash-service-config.json <!TOKEN!>",
            "cmd_path" : "C:/Users/dc/Documents/Projects/dc/dash_code/py_server"
        }
    }
}
```

### 1.2 ^^Definitions^^

#### 1.2.1 Main

| Variable | Definition |
| ------ | ------ |
| **`port`** | Fixed port number. |
| **`cert_filename`** | Fixed certification filename. |
| **`key_filename`** | Fixed certification key filename. |
| **`dh_params_filename`** | Fixed parameter filename. |
| **`robot_register_native_cert`** |  If you registed with register_bot_native, the data will be encrypted. Always set this variable to true. |
| **`active_IP_idx`** | Selects the IP address you will send to the backend cloud service for robot discovery. This is an integer index ( from 0 to N ), based on the IP addresses available on your system. When the rest service starts up, you should see a list. Set the value to the appropriate index you want. This index will map the the IP which the clients will try to connect to. |
| **`preferred_IP`** | Selects your preferred IP from the list of IPs. Specify the IP as a string in this case. |

---

#### 1.2.2 d.ASH Server Commands

| Variable | Definition |
| ------ | ------ |
| **`cmd_str`** | Sets command to run d.ASH server. |
| **`cmd_path`** | Sets command path. |
