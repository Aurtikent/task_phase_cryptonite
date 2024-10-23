#Perceibing Permissions

### Flags and Writeups

1) pwn.college{wctLmIPJzr_psWO4jI7Is8whPOD.dFTM2QDL2gTN0czW}
    - `chown` is used to change the owner of the files, 
    - `chown hacker /flag` changes the owner of file to hacker so we can as 'hacker' user can read it.  
    - ` cat /flag` gives us the flag. 
2) pwn.college{UYSZPWYxsoB9t-KI4iplcBEVXAb.dFzNyUDL2gTN0czW}
    - `chgrp` is used to change the group ownership of files
    - `chgrp hacker /flag` 
    - `cat /flag` will give us the flag. 
3) pwn.college{QkQLfaFLGnZpN9u7OsKHuFN1kLN.dJzNyUDL2gTN0czW}
    - use `id` to find out your group name `<grp30369>` in this case.
    - `chgrp grp30369 /flag`
    - `cat /flag` will give us the flag. 
4) pwn.college{Yn5TKvMyb6vq_lfMUXD6N9WlpbS.dNzNyUDL2gTN0czW}
    - `chmod` to change file perms. 
    - `chmod a+r /flag`gives read perm to all user, groups,and others
    - `cat /flag` will give you the flag. 
5) pwn.college{4k2-3la4zPirkxFrcMiKl67oYGQ.dJTM2QDL2gTN0czW}
    - `chmod +x /challenge/run` to give it execute perms
    - `/challenge/run` will give the flag. 
6) pwn.college{QhROrWN7Ld9mZtbv_rYIKkRFeoU.dBTM2QDL2gTN0czW}
    - go through various rounds of chmodding a file setting up permissions for it. 
    - `chmod +r /flag` change the perm of the flag. 
    - `cat /flag` to give us the flag. 
7) pwn.college{43TJ08P0uw3UdszK7R0YRJoHFWh.dNTM5QDL2gTN0czW}
    - Go through Various rounds advance chmodding for a file
    - `chmod +r /flag` change the perm of the flag. 
    - `cat /flag` to give us the flag. 
8) pwn.college{wETgeYYZHX4nRT_al50W5DnOmBr.dNTM2QDL2gTN0czW}
    - Set SUID bit for /challenge/getroot with:
    - `chmod +s /challenge/getroot`
    - run program which spawns a root shell, `cat /flag`

