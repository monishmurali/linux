
# CMPE 283 Assignment 3


  #Question 1.
 Assignment done by myself.
 
 #Question 2:
 => steps for assignment 3:
 1. Create Vm instance in Google cloud and enabled nested VM.
 2. Fork Linux Github repo.
 3. Build Kernel.
 
 <img width="352" alt="afterkernelbuild" src="https://user-images.githubusercontent.com/59603371/205843934-8ef25a02-6e60-43d0-bc37-55236f00e4bf.PNG">
 
 4. make code changes in both cpuid.c and vmx.c
 5. using sudo make modules.
 6. kvm module is loaded using lsmod. 
 7. kvm is removed using rmmod kvm_intel.
 8. Loaded KVM using Sudo modprobe kvm and sudo modprobe kvm_intel command
 9. created nested vm in gcp to test. make 2 terminals gcp vm terminal and nested vm terminal open.
 10. created new test script and tested
 
 
 <img width="492" alt="J_modules" src="https://user-images.githubusercontent.com/59603371/207237548-57fb9f29-3f78-45b8-bdb5-a20c872bf8ac.PNG">

 
 <img width="725" alt="Output" src="https://user-images.githubusercontent.com/59603371/207237843-1e31e868-2ec5-4bd3-8561-eac3366929ac.PNG">
 

 
 <img width="595" alt="output_0x4ffffff_exitno _totalexit" src="https://user-images.githubusercontent.com/59603371/207237929-017cb8c2-fde8-4f21-bbd2-03509fa8b9b6.PNG">
 
 
 <img width="675" alt="output_0x4ffffffe" src="https://user-images.githubusercontent.com/59603371/207238028-26c1068b-d089-4233-a92e-e7e99f35dbe8.PNG">
 
 
 
 <img width="444" alt="output_3ques" src="https://user-images.githubusercontent.com/59603371/207238099-228efaf5-00da-47db-aadf-eeb3caf9e90b.PNG">
 
 
 #Questioon 3:
Comment on the frequency of exits – does the number of exits increase at a stable rate? Or are theremore exits performed during certain VM operations? Approximately how many exits does a full VM boot entail?

 for HLT(10) and CPUID(12) the number of exits increased at a stable rate.
 
 
 output:
 
 <img width="444" alt="output_3ques" src="https://user-images.githubusercontent.com/59603371/207238700-49966e5b-90b5-46a5-be23-63eb4803a170.PNG">
 
 
 #Question 4:
 
 Most Frequently Called Exits are:
 
 Exit#30 - IO_Instruction,
 Exit#49 - EPT_MISCONFIG,
 Exit#28 - CR_ACCESS
 
Least frequently called exists are:

Exit#54 - WBINVD,
Exit#29 - DR_ACCESS,
Exit #0 - Expection_NMI

<img width="473" alt="ques4" src="https://user-images.githubusercontent.com/59603371/207239864-ff2b8955-2c64-4b9e-bde4-fad07ba57512.PNG">


# steps for assignment 2:

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















