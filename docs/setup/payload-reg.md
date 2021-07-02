# Payload Registration

Before running the d.ASH SDK, please make sure that all of your credentials have been set up correctly. This means using the right username and the right password. This section of the d.ASH SDK documentation provides details about setting up credentials for the d.ASH server, your robot, and d.ASH autonomy. Files in this section can be found in the folder `registration`:

```
dash-sdk/
└─ registration
    └─ set_spot_cred
    └─ register_payload
    └─ set_autonomy_cred
    
```

### 2.1 ^^d.ASH Server Credentials^^

To set up the local credentials for the d.ASH server, you will need to run the file `set_spot_cred`. Run the following command replacing `<USERNAME>` with your chosen username and  `<PASSWORD>` with your chosen password.

```
./set_spot_cred -u <USERNAME> -p <PASSWORD>
```

For example, if your username is `user123` and your password is `pw123`, your command would look like this:
``` python
./set_spot_cred -u user123 -p pw123
```

!!! tip "Username in Robot Configuration"
    Please ensure that the username for the d.ASH server is the same as the one defined in the robot configuration file - [`robot_config.json`](/dash-sdk/sdk-config/robot-config). That is, you would replace `<USERNAME>` with your chosen username in `"username" : "<USERNAME>"`.

--- 

### 2.2 ^^Robot Registration^^

To register the payload computer with d.ASH's backend system, you will need to run the file `register_payload`. However, you will first need to configure the [`register_payload_config.json`](/dash-sdk/sdk-config/register-bot) found in the `\dash-sdk\configs` folder of the SDK. Set `<ROBOT_NAME>` to any name you like, and set `<DC_USERNAME>` to your dConstruct cloud admin username. 

For example, if your robot name is `robot1` and your cloud admin user name is `user123`, your `register_payload_config.json` would look like this:

```
{
    RobotName: robot1,
    RobotUserName: user123
}
```

Now, run the following command to register your robot, replacing `<PATH_TO_SDK>` with your local path to the d.ASH SDK.

```
./register_payload -i <PATH_TO_SDK>/dash_sdk/configs/register_payload_config
```

---

### 2.3 ^^d.ASH Autonomy Credentials^^

To set up the local credentials for d.ASH autonomy, you will need to run the file  `set_autonomy_cred`. Run the following command replacing `<USERNAME>` with your cloud admin username. 

``` python
cd ./set_auto_cred/build
./set_autonomy_cred -u <USERNAME> 
```
For example, if your username is `user123`, your command would look like this:
``` python
cd ./set_auto_cred/build
./set_autonomy_cred -u user123
```
You will then be prompted to enter a password, which will match your cloud admin password. Enter