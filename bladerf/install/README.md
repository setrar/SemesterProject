

```
sudo yum install gcc gcc-c++ make cmake libusb1-devel ncurses-devel
```
> Returns
```powershell
Updating Subscription Management repositories.
Last metadata expiration check: 2:28:56 ago on Sat 09 Nov 2024 12:33:13 PM CET.
Package gcc-11.3.1-4.3.el9.x86_64 is already installed.
Package gcc-c++-11.3.1-4.3.el9.x86_64 is already installed.
Package make-1:4.3-7.el9.x86_64 is already installed.
Package cmake-3.20.2-8.el9.x86_64 is already installed.
Package libusbx-devel-1.0.26-1.el9.x86_64 is already installed.
Package ncurses-devel-6.2-8.20210508.el9.x86_64 is already installed.
Dependencies resolved.
======================================================================================================================================================================
 Package                                Architecture               Version                                 Repository                                            Size
======================================================================================================================================================================
Upgrading:
 cmake                                  x86_64                     3.26.5-2.el9                            rhel-9-for-x86_64-appstream-rpms                     8.7 M
 cmake-data                             noarch                     3.26.5-2.el9                            rhel-9-for-x86_64-appstream-rpms                     2.4 M
 cmake-filesystem                       x86_64                     3.26.5-2.el9                            rhel-9-for-x86_64-appstream-rpms                      23 k
 cmake-rpm-macros                       noarch                     3.26.5-2.el9                            rhel-9-for-x86_64-appstream-rpms                      12 k
 cpp                                    x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-appstream-rpms                      11 M
 gcc                                    x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-appstream-rpms                      32 M
 gcc-c++                                x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-appstream-rpms                      13 M
 gcc-gfortran                           x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-appstream-rpms                      13 M
 gcc-plugin-annobin                     x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-appstream-rpms                      49 k
 libgcc                                 x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-baseos-rpms                         95 k
 libgfortran                            x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-baseos-rpms                        804 k
 libgomp                                x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-baseos-rpms                        270 k
 libquadmath                            x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-baseos-rpms                        197 k
 libquadmath-devel                      x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-appstream-rpms                      38 k
 libstdc++                              x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-baseos-rpms                        747 k
 libstdc++-devel                        x86_64                     11.4.1-3.el9                            rhel-9-for-x86_64-appstream-rpms                     2.4 M
 make                                   x86_64                     1:4.3-8.el9                             rhel-9-for-x86_64-baseos-rpms                        541 k
 ncurses                                x86_64                     6.2-10.20210508.el9                     rhel-9-for-x86_64-baseos-rpms                        410 k
 ncurses-base                           noarch                     6.2-10.20210508.el9                     rhel-9-for-x86_64-baseos-rpms                         99 k
 ncurses-c++-libs                       x86_64                     6.2-10.20210508.el9                     rhel-9-for-x86_64-appstream-rpms                      39 k
 ncurses-devel                          x86_64                     6.2-10.20210508.el9                     rhel-9-for-x86_64-appstream-rpms                     732 k
 ncurses-libs                           x86_64                     6.2-10.20210508.el9                     rhel-9-for-x86_64-baseos-rpms                        332 k

Transaction Summary
======================================================================================================================================================================
Upgrade  22 Packages

Total download size: 86 M
Is this ok [y/N]: y
Downloading Packages:
(1/22): ncurses-c++-libs-6.2-10.20210508.el9.x86_64.rpm                                                                                79 kB/s |  39 kB     00:00    
(2/22): ncurses-devel-6.2-10.20210508.el9.x86_64.rpm                                                                                  851 kB/s | 732 kB     00:00    
(3/22): cmake-filesystem-3.26.5-2.el9.x86_64.rpm                                                                                       50 kB/s |  23 kB     00:00    
(4/22): cmake-3.26.5-2.el9.x86_64.rpm                                                                                                 8.4 MB/s | 8.7 MB     00:01    
(5/22): gcc-plugin-annobin-11.4.1-3.el9.x86_64.rpm                                                                                    139 kB/s |  49 kB     00:00    
(6/22): libstdc++-devel-11.4.1-3.el9.x86_64.rpm                                                                                       5.9 MB/s | 2.4 MB     00:00    
(7/22): cmake-data-3.26.5-2.el9.noarch.rpm                                                                                            4.6 MB/s | 2.4 MB     00:00    
(8/22): cmake-rpm-macros-3.26.5-2.el9.noarch.rpm                                                                                       23 kB/s |  12 kB     00:00    
(9/22): cpp-11.4.1-3.el9.x86_64.rpm                                                                                                    18 MB/s |  11 MB     00:00    
(10/22): gcc-c++-11.4.1-3.el9.x86_64.rpm                                                                                               27 MB/s |  13 MB     00:00    
(11/22): libquadmath-devel-11.4.1-3.el9.x86_64.rpm                                                                                    211 kB/s |  38 kB     00:00    
(12/22): gcc-gfortran-11.4.1-3.el9.x86_64.rpm                                                                                          27 MB/s |  13 MB     00:00    
(13/22): gcc-11.4.1-3.el9.x86_64.rpm                                                                                                   53 MB/s |  32 MB     00:00    
(14/22): ncurses-6.2-10.20210508.el9.x86_64.rpm                                                                                       793 kB/s | 410 kB     00:00    
(15/22): ncurses-base-6.2-10.20210508.el9.noarch.rpm                                                                                  189 kB/s |  99 kB     00:00    
(16/22): libgcc-11.4.1-3.el9.x86_64.rpm                                                                                               513 kB/s |  95 kB     00:00    
(17/22): ncurses-libs-6.2-10.20210508.el9.x86_64.rpm                                                                                  1.6 MB/s | 332 kB     00:00    
(18/22): libgomp-11.4.1-3.el9.x86_64.rpm                                                                                              1.4 MB/s | 270 kB     00:00    
(19/22): libstdc++-11.4.1-3.el9.x86_64.rpm                                                                                            3.7 MB/s | 747 kB     00:00    
(20/22): libgfortran-11.4.1-3.el9.x86_64.rpm                                                                                          4.1 MB/s | 804 kB     00:00    
(21/22): libquadmath-11.4.1-3.el9.x86_64.rpm                                                                                          344 kB/s | 197 kB     00:00    
(22/22): make-4.3-8.el9.x86_64.rpm                                                                                                    1.1 MB/s | 541 kB     00:00    
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                                                  25 MB/s |  86 MB     00:03     
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :                                                                                                                                              1/1 
  Upgrading        : libgcc-11.4.1-3.el9.x86_64                                                                                                                  1/44 
  Running scriptlet: libgcc-11.4.1-3.el9.x86_64                                                                                                                  1/44 
  Upgrading        : libstdc++-11.4.1-3.el9.x86_64                                                                                                               2/44 
  Upgrading        : libquadmath-11.4.1-3.el9.x86_64                                                                                                             3/44 
  Upgrading        : make-1:4.3-8.el9.x86_64                                                                                                                     4/44 
  Upgrading        : cmake-rpm-macros-3.26.5-2.el9.noarch                                                                                                        5/44 
  Upgrading        : cmake-filesystem-3.26.5-2.el9.x86_64                                                                                                        6/44 
  Upgrading        : libgfortran-11.4.1-3.el9.x86_64                                                                                                             7/44 
  Upgrading        : libstdc++-devel-11.4.1-3.el9.x86_64                                                                                                         8/44 
  Upgrading        : libgomp-11.4.1-3.el9.x86_64                                                                                                                 9/44 
  Upgrading        : ncurses-base-6.2-10.20210508.el9.noarch                                                                                                    10/44 
  Upgrading        : ncurses-libs-6.2-10.20210508.el9.x86_64                                                                                                    11/44 
  Upgrading        : ncurses-c++-libs-6.2-10.20210508.el9.x86_64                                                                                                12/44 
  Upgrading        : cmake-data-3.26.5-2.el9.noarch                                                                                                             13/44 
  Upgrading        : cmake-3.26.5-2.el9.x86_64                                                                                                                  14/44 
  Upgrading        : cpp-11.4.1-3.el9.x86_64                                                                                                                    15/44 
  Upgrading        : gcc-11.4.1-3.el9.x86_64                                                                                                                    16/44 
  Running scriptlet: gcc-11.4.1-3.el9.x86_64                                                                                                                    16/44 
  Upgrading        : libquadmath-devel-11.4.1-3.el9.x86_64                                                                                                      17/44 
  Upgrading        : gcc-gfortran-11.4.1-3.el9.x86_64                                                                                                           18/44 
  Upgrading        : gcc-plugin-annobin-11.4.1-3.el9.x86_64                                                                                                     19/44 
  Running scriptlet: gcc-plugin-annobin-11.4.1-3.el9.x86_64                                                                                                     19/44 
  Upgrading        : gcc-c++-11.4.1-3.el9.x86_64                                                                                                                20/44 
  Upgrading        : ncurses-devel-6.2-10.20210508.el9.x86_64                                                                                                   21/44 
  Upgrading        : ncurses-6.2-10.20210508.el9.x86_64                                                                                                         22/44 
  Cleanup          : ncurses-devel-6.2-8.20210508.el9.x86_64                                                                                                    23/44 
  Cleanup          : cmake-3.20.2-8.el9.x86_64                                                                                                                  24/44 
  Cleanup          : ncurses-c++-libs-6.2-8.20210508.el9.x86_64                                                                                                 25/44 
  Cleanup          : gcc-gfortran-11.3.1-4.3.el9.x86_64                                                                                                         26/44 
  Cleanup          : libgfortran-11.3.1-4.3.el9.x86_64                                                                                                          27/44 
  Cleanup          : gcc-c++-11.3.1-4.3.el9.x86_64                                                                                                              28/44 
  Cleanup          : cmake-data-3.20.2-8.el9.noarch                                                                                                             29/44 
  Cleanup          : ncurses-6.2-8.20210508.el9.x86_64                                                                                                          30/44 
  Cleanup          : gcc-plugin-annobin-11.3.1-4.3.el9.x86_64                                                                                                   31/44 
  Running scriptlet: gcc-plugin-annobin-11.3.1-4.3.el9.x86_64                                                                                                   31/44 
  Cleanup          : libquadmath-devel-11.3.1-4.3.el9.x86_64                                                                                                    32/44 
  Cleanup          : libstdc++-devel-11.3.1-4.3.el9.x86_64                                                                                                      33/44 
  Cleanup          : cmake-filesystem-3.20.2-8.el9.x86_64                                                                                                       34/44 
  Cleanup          : cmake-rpm-macros-3.20.2-8.el9.noarch                                                                                                       35/44 
  Cleanup          : gcc-11.3.1-4.3.el9.x86_64                                                                                                                  36/44 
  Cleanup          : libstdc++-11.3.1-4.3.el9.x86_64                                                                                                            37/44 
  Cleanup          : libquadmath-11.3.1-4.3.el9.x86_64                                                                                                          38/44 
  Cleanup          : ncurses-libs-6.2-8.20210508.el9.x86_64                                                                                                     39/44 
  Cleanup          : ncurses-base-6.2-8.20210508.el9.noarch                                                                                                     40/44 
  Cleanup          : libgcc-11.3.1-4.3.el9.x86_64                                                                                                               41/44 
  Running scriptlet: libgcc-11.3.1-4.3.el9.x86_64                                                                                                               41/44 
  Cleanup          : cpp-11.3.1-4.3.el9.x86_64                                                                                                                  42/44 
  Cleanup          : libgomp-11.3.1-4.3.el9.x86_64                                                                                                              43/44 
  Cleanup          : make-1:4.3-7.el9.x86_64                                                                                                                    44/44 
  Running scriptlet: make-1:4.3-7.el9.x86_64                                                                                                                    44/44 
  Verifying        : ncurses-devel-6.2-10.20210508.el9.x86_64                                                                                                    1/44 
  Verifying        : ncurses-devel-6.2-8.20210508.el9.x86_64                                                                                                     2/44 
  Verifying        : ncurses-c++-libs-6.2-10.20210508.el9.x86_64                                                                                                 3/44 
  Verifying        : ncurses-c++-libs-6.2-8.20210508.el9.x86_64                                                                                                  4/44 
  Verifying        : cmake-3.26.5-2.el9.x86_64                                                                                                                   5/44 
  Verifying        : cmake-3.20.2-8.el9.x86_64                                                                                                                   6/44 
  Verifying        : cmake-filesystem-3.26.5-2.el9.x86_64                                                                                                        7/44 
  Verifying        : cmake-filesystem-3.20.2-8.el9.x86_64                                                                                                        8/44 
  Verifying        : gcc-plugin-annobin-11.4.1-3.el9.x86_64                                                                                                      9/44 
  Verifying        : gcc-plugin-annobin-11.3.1-4.3.el9.x86_64                                                                                                   10/44 
  Verifying        : libstdc++-devel-11.4.1-3.el9.x86_64                                                                                                        11/44 
  Verifying        : libstdc++-devel-11.3.1-4.3.el9.x86_64                                                                                                      12/44 
  Verifying        : cmake-data-3.26.5-2.el9.noarch                                                                                                             13/44 
  Verifying        : cmake-data-3.20.2-8.el9.noarch                                                                                                             14/44 
  Verifying        : cmake-rpm-macros-3.26.5-2.el9.noarch                                                                                                       15/44 
  Verifying        : cmake-rpm-macros-3.20.2-8.el9.noarch                                                                                                       16/44 
  Verifying        : cpp-11.4.1-3.el9.x86_64                                                                                                                    17/44 
  Verifying        : cpp-11.3.1-4.3.el9.x86_64                                                                                                                  18/44 
  Verifying        : gcc-c++-11.4.1-3.el9.x86_64                                                                                                                19/44 
  Verifying        : gcc-c++-11.3.1-4.3.el9.x86_64                                                                                                              20/44 
  Verifying        : gcc-gfortran-11.4.1-3.el9.x86_64                                                                                                           21/44 
  Verifying        : gcc-gfortran-11.3.1-4.3.el9.x86_64                                                                                                         22/44 
  Verifying        : libquadmath-devel-11.4.1-3.el9.x86_64                                                                                                      23/44 
  Verifying        : libquadmath-devel-11.3.1-4.3.el9.x86_64                                                                                                    24/44 
  Verifying        : gcc-11.4.1-3.el9.x86_64                                                                                                                    25/44 
  Verifying        : gcc-11.3.1-4.3.el9.x86_64                                                                                                                  26/44 
  Verifying        : ncurses-6.2-10.20210508.el9.x86_64                                                                                                         27/44 
  Verifying        : ncurses-6.2-8.20210508.el9.x86_64                                                                                                          28/44 
  Verifying        : ncurses-base-6.2-10.20210508.el9.noarch                                                                                                    29/44 
  Verifying        : ncurses-base-6.2-8.20210508.el9.noarch                                                                                                     30/44 
  Verifying        : ncurses-libs-6.2-10.20210508.el9.x86_64                                                                                                    31/44 
  Verifying        : ncurses-libs-6.2-8.20210508.el9.x86_64                                                                                                     32/44 
  Verifying        : libgcc-11.4.1-3.el9.x86_64                                                                                                                 33/44 
  Verifying        : libgcc-11.3.1-4.3.el9.x86_64                                                                                                               34/44 
  Verifying        : libgomp-11.4.1-3.el9.x86_64                                                                                                                35/44 
  Verifying        : libgomp-11.3.1-4.3.el9.x86_64                                                                                                              36/44 
  Verifying        : libquadmath-11.4.1-3.el9.x86_64                                                                                                            37/44 
  Verifying        : libquadmath-11.3.1-4.3.el9.x86_64                                                                                                          38/44 
  Verifying        : libstdc++-11.4.1-3.el9.x86_64                                                                                                              39/44 
  Verifying        : libstdc++-11.3.1-4.3.el9.x86_64                                                                                                            40/44 
  Verifying        : make-1:4.3-8.el9.x86_64                                                                                                                    41/44 
  Verifying        : make-1:4.3-7.el9.x86_64                                                                                                                    42/44 
  Verifying        : libgfortran-11.4.1-3.el9.x86_64                                                                                                            43/44 
  Verifying        : libgfortran-11.3.1-4.3.el9.x86_64                                                                                                          44/44 
Installed products updated.

Upgraded:
  cmake-3.26.5-2.el9.x86_64                            cmake-data-3.26.5-2.el9.noarch                           cmake-filesystem-3.26.5-2.el9.x86_64                 
  cmake-rpm-macros-3.26.5-2.el9.noarch                 cpp-11.4.1-3.el9.x86_64                                  gcc-11.4.1-3.el9.x86_64                              
  gcc-c++-11.4.1-3.el9.x86_64                          gcc-gfortran-11.4.1-3.el9.x86_64                         gcc-plugin-annobin-11.4.1-3.el9.x86_64               
  libgcc-11.4.1-3.el9.x86_64                           libgfortran-11.4.1-3.el9.x86_64                          libgomp-11.4.1-3.el9.x86_64                          
  libquadmath-11.4.1-3.el9.x86_64                      libquadmath-devel-11.4.1-3.el9.x86_64                    libstdc++-11.4.1-3.el9.x86_64                        
  libstdc++-devel-11.4.1-3.el9.x86_64                  make-1:4.3-8.el9.x86_64                                  ncurses-6.2-10.20210508.el9.x86_64                   
  ncurses-base-6.2-10.20210508.el9.noarch              ncurses-c++-libs-6.2-10.20210508.el9.x86_64              ncurses-devel-6.2-10.20210508.el9.x86_64             
  ncurses-libs-6.2-10.20210508.el9.x86_64             

Complete!
```

# References

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

:x: This didn't work

To install the bladeRF CLI (command-line interface) on Red Hat, follow these steps:
	1.	Enable the EPEL Repository: Since the Extra Packages for Enterprise Linux (EPEL) repository may have dependencies for bladeRF, you may want to enable it:

sudo yum install epel-release


	2.	Download the Nuand Repository: Nuand provides pre-built packages for bladeRF on Red Hat and CentOS, so you can add the Nuand repository directly.

sudo dnf config-manager --add-repo https://nuand.com/yum/el7/nuand.repo


	3.	Install the bladeRF CLI:

sudo dnf install bladerf


	4.	Verify Installation: After installation, check if bladeRF CLI is working by typing:

bladerf-cli -h



If you encounter any missing dependencies or repository issues, you may need to install manually from the source or check the bladeRF documentation for specific Red Hat instructions.
