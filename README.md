# CMPE 283 Assignment 1

## Question 1: 

## Question 2: Steps followed in the assignment

1. Installed VM Fusion for MAC OS

2. Installed Ubuntu v20.04 

3. Enabled hypervisior option for nested virtualization capabilities in the settings during ubuntu installation

4. Cloned the torvarlds linux repo using ``` git clone git@github.com:torvalds/linux.git ```

5. Added a new directory cmpe 283 inside the cloned repo and copy both the cmpe283-1.c and Makefile to this new cmpe283 folder

6. Edited the cmpe283-1.c inside the cmpe283 folder with all the MSRs needed to complete the assignment
  * Pinbased Controls
  * Primary Processor based controls
  * Secondary Processor based controls if available
  * Entry Controls
  * Exit Controls

7. Buit the modules by running ```make```

8. Run ```sudo insmod cmpe283-1.ko``` to insert the modules into the linux kernel. Execution starts at init_module()

9. Run ```sudo rmmod cmpe283-1``` to remove the modules from the linux kernel. Clean up of modules is performed by cleanup_module()

10. Output can be checked by executing ```dmesg``` and copied the result to **result.txt**
