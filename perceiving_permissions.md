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
6) 
