## Steps to change the MAC Address in Kali Linux

* Disable the interface you want to change the MAC address for.
* Change the MAC address
* Enable the interface.

<hr>

# In Action

Follow the steps and run the given commands: 

* Disable the interface : ```ifconfig eth0 down```

    * Here eth0 is the name of the interface we want to change the MAC for.

* Change the MAC : 
```ifconfig eth0 hw ether 00:11:22:33:44:55```
    * Here 'hw' stands for hardware interface and '00:11:22:33:44:55' is the fake MAC that we have given to change the MAC. The MAC address will be changed to this given random address.

* Enable the interface : ```ifconfig eth0 up```

Now simply run the command ```ifconfig``` and check!!! . The MAC address will be changes........

<hr>