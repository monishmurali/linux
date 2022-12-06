Linux kernel
============

steps for assignment 2:

1. create vm instance

created vm instance of ubuntu with bootspace 150gb and enabled nested vm.

2.  fork linux github repo


![image](https://user-images.githubusercontent.com/59603371/205843398-cac24460-a734-4884-95c2-2b45973f7d87.png)



3. build kernel


After kernel was build



<img width="352" alt="afterkernelbuild" src="https://user-images.githubusercontent.com/59603371/205843934-8ef25a02-6e60-43d0-bc37-55236f00e4bf.PNG">



4. kvm module is loaded using lsmod. 

5. kvm is removed using rmmod kvm_intel.
 
6. Loaded KVM using Sudo modprobe kvm and sudo modprobe kvm_intel command



![image](https://user-images.githubusercontent.com/59603371/205850082-1ad6ae8c-9048-4d61-9f0a-14d75a297d41.png)


![image](https://user-images.githubusercontent.com/59603371/205850168-31dee037-a966-4b32-8bf1-17c1d50d3c53.png)


![image](https://user-images.githubusercontent.com/59603371/205850230-bf9c3561-691c-4faa-b25f-e9c4596754d2.png)


![image](https://user-images.githubusercontent.com/59603371/205850379-bbe3a28a-1cf4-43a6-b057-486244de4670.png)


![image](https://user-images.githubusercontent.com/59603371/205850454-970f958e-494e-423b-9c38-71de1e714fbd.png)















