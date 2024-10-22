# Processes and Jobs
### Writeups and Flags, 

1) pwn.college{0OSe7atsPFPfa4FJVMrZ_4oI7AF.dhzM4QDL2gTN0czW}
    - ps displays processes in the terminal
    - `ps -ef` will give 'every process' in 'full' format. 

2) pwn.college{E6kp6vPXaA9P2H0ORZi3oFKyHFW.dJDN4QDL2gTN0czW}
    -'kill' is used to kill a process
    - check PID with `ps -ef`
    - `kill <PID>`
//TODO: insert image here. 

3) pwn.college{cBCKM2D6lmFQhv1jM4FcRx_QO_X.dNDN4QDL2gTN0czW}
    - `/challenge/run`
    - press ctrl +c to give the flag. 
4) pwn.college{0zfSyjIh30EDWFZVa4EFF1aylBs.dVDN4QDL2gTN0czW}
    - `/challenge/run`
    - ctrl + z to 'suspend' it background
    - `/challenge/run` again to give us the flag. 
5) pwn.college{guma9-NDkL0FmqVF4CgOWrcPRo9.dZDN4QDL2gTN0czW}
    - `/challenge/run` for the challenges,
    - Ctrl + Z to shift it to the background suspended
    - `fg` to resume it again and give us the flag.
6) pwn.college{A_OwIrDPRHHDmEW8W1Gr1dgC_oU.ddDN4QDL2gTN0czW}
    - 'bg' resumes stopped background processes
    - run `/challenge/run` then  'ctrl +z' 
    - `bg` 
    - `/challenge/run` will print the flag.  
7)  pwn.college{oDnHg9mkivT6txu-KVNGiL5qML2.dhDN4QDL2gTN0czW}
    -`/challenge/run`, ctrl +z
    - `bg`
    - `fg` gives us the flag. 
8) pwn.college{81EHu_ylPwmikBoHF4s-PCRQHT7.dlDN4QDL2gTN0czW}
    - & will start the process in the background with suspending, 
    - `/challenge/run &` will give us the flag. 
9) pwn.college{cNLYp9hQ7-6dPTFv4x2paGNVe6N.dljN4UDL2gTN0czW}
    - `$?` to get the code. 
    - `/challenge/get-code` program exits with a error code
    - `echo $?` to get the code
    - `/challenge/submit-code 242` will give the flag. 
