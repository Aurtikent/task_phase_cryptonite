# Comprehending_commands

## Flags and notes

1) pwn.college{0G0f_M2qaH9SonbfxKpmbud_CXc.dFzN1QDL2gTN0czW}
    - `cat flag` gives us the flag. 
2) pwn.college{EIGSN9sK9O4TUozb0dOaY0El0gu.dlTM5QDL2gTN0czW}
    `cat /flag` gives the flag. 
3)pwn.college{sQj_tNj8hSwxmFFHTjDxQiV1vwv.dBjM5QDL2gTN0czW}
    - running `cd /` gives us the directory where flag is located. 
    - `cat /opt/busybox/fs/flag` gives us the flag. 
4) pwn.college{gbiF-K9khCxEZ4SkQhi68AHYpNk.ddTM4QDL2gTN0czW}
    - ` grep pwn.college /challenge/data.txt ` gives us the flag,
    - grep matchs the 'pwn.college' string from 'data.txt' 
5)pwn.college{Y5seNzl0SjFzG-79LqhgupOQcIw.dhjM4QDL2gTN0czW}
    - `cd /challenge` to get to the directory
    - `ls` lists the files in the directory
    - `./10397-renamed-run-31044` is the renamed run, running the command gives us the flag. 
6)pwn.college{sN2HwzVvTwxZFwDUTP5b6Q8o8Ai.dBzM4QDL2gTN0czW}
    - `touch /tmp/pwn`
    - `touch /tmp/college`
    - the above two commanbds create files needed, 
    - `/challenge/run` prints the commands, 
7) pwn.college{MJIiIEwhQQtZX84u1no_wJkmNa4.dZTOwUDL2gTN0czW}
    - `rm delete_me` removes the the file 'delete_me'
    - `/challenge/check` prints the flag. 
8)pwn.college{kj2rey2xNdH0zUUXXaDCvSnsupu.dBTN4QDL2gTN0czW}
    - `cd /` as told in the description
    - ` ls -a` prints the all the files including hidden files,     
    -  `cat  .flag-2023110815938` prints the flag. 
9)pwn.college{wgaaLElgP6TDegWyR3bFBzg-XAA.dljM4QDL2gTN0czW} 
    - use a combination of `ls -a <direcotryname> ` and `cat <directoryname>/<cluefile>` repeatedly
    - will need to sometimes cd into the particular directory to read the next directory,
    - continue the process till you find the last directory printing the flag. 
10) pwn.college{slkBBH_a_Q2YuG6ORWjMulwZtpC.dFzM4QDL2gTN0czW}
    - `mkdir /tmp/pwn` will make a directory
    - `touch /tmp/pwn/college` will make a file in the directory created as prescribed.
    - `/challenge/run` will print the flag.
11) pwn.college{4lh9xyDLBoHf8Omtuad5F9_7cNO.dJzM4QDL2gTN0czW}
    - `find / -name flag -type f` will print the path to flag. 
    - '/' tells the directory to search 
    - -name is the name of the file
    - -type f specifies that we need to search files by default find searches for directories. 
12) pwn.college{sYnfQ2lXjhllgs6dA2kgVYIdOwb.dlTM1UDL2gTN0czW}
    - we need create a symlink to the /flag directory
    - '/challenge/catflag' will read the the /home/hacker/not-the-flag file,
    - `ln -s /flag /home/hacker/not-the-flag` will create the soft link to not-the-flag file
    - `/challenge/catflag` copy and read out the flag from 'not-the-flag' thus printing the flag to the terminal. 



