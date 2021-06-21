# Configuring Spot

This section of the d.ASH SDK documentation provides details about setting up Spot with the d.ASH SDK. To configure Spot, you will need to set up on the robot itself and on your personal computer. For further enquiries of setting up Spot, follow [Boston Dynamics Documentation](https://www.bostondynamics.com/sites/default/files/inline-files/spot-system-administration.pdf).

### 1.1 ^^Setting Up On Spot^^
By default, user and admin credentials are printed on the label of the robot's battery compartment. Otherwise, you can create your own account through the admin console by creating a user with admin privileges. Check out [Boston Dynamics Documentation](https://www.bostondynamics.com/sites/default/files/inline-files/spot-system-administration.pdf) for more information on how to do so.

!!! tip "Remember your credentials!"
    Remember your Spot credentials as you will need those same credentials to set up the next section on your personal computer.

---

### 1.2 ^^Setting Up On PC^^
By default, the Spot robot IP address is `10.0.0.3`. If you have more than one Spot robot, refer to the [Boston Dynamics Documentation](https://www.bostondynamics.com/sites/default/files/inline-files/spot-system-administration.pdf) to use the admin console to change the default IP of additional robots to avoid address conflicts.

You'll need to configure a static IP address for your computer to use an address within the range `10.0.0.X` where `X` may be any integer from 2 to 254, except 3 (which is the Spot's IP). For example, an appropriate static IP address for your compute could be `10.0.0.100`. You will then be asked to enter a valid admin or operator username and password. These credentials will match the credentials on Spot's battery compartment.