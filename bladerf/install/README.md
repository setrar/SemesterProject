

```
sudo yum install epel-release
```
> Returns
```powershell
Updating Subscription Management repositories.
Last metadata expiration check: 1:56:01 ago on Sat 09 Nov 2024 12:33:13 PM CET.
Package epel-release-8-19.el8.noarch is already installed.
Dependencies resolved.
======================================================================================================================================================================
 Package                                     Architecture                          Version                                  Repository                           Size
======================================================================================================================================================================
Upgrading:
 epel-release                                noarch                                8-21.el8                                 epel                                 24 k

Transaction Summary
======================================================================================================================================================================
Upgrade  1 Package

Total download size: 24 k
Is this ok [y/N]: y
Downloading Packages:
epel-release-8-21.el8.noarch.rpm                                                                                                      570 kB/s |  24 kB     00:00    
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                                                 103 kB/s |  24 kB     00:00     
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :                                                                                                                                              1/1 
  Upgrading        : epel-release-8-21.el8.noarch                                                                                                                 1/2 
  Running scriptlet: epel-release-8-21.el8.noarch                                                                                                                 1/2 
  Cleanup          : epel-release-8-19.el8.noarch                                                                                                                 2/2 
  Running scriptlet: epel-release-8-19.el8.noarch                                                                                                                 2/2 
  Verifying        : epel-release-8-21.el8.noarch                                                                                                                 1/2 
  Verifying        : epel-release-8-19.el8.noarch                                                                                                                 2/2 
Installed products updated.

Upgraded:
  epel-release-8-21.el8.noarch                                                                                                                                        

Complete!
```
