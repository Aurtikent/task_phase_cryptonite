# Pondering Paths

## Notes and Flags

1) pwn.college{wehc1KpwRtQE2yezdwokUHnDjCu.dhzN5QDL2gTN0czW}
    - `/pwn` ran the command to get the flag.   

2) pwn.college{wF9kQ3s2HorjVh3lEur2SDCJhue.dVDN1QDL2gTN0czW}
    - ran with absolute path to the command tot get the flag
    - `/challenge/run`
3) pwn.college{8DEJnUhuJx_W1CuXXIYdF5veKO8.dZDN1QDL2gTN0czW}    
    - use `cd /usr/share/zoneinfo/posix/Asia` to change directory to run the binary
    - `/challenge/run` gives the flag.
4) pwn.college{kPsgTtKceZeJDC-sRbKzLvJd0B4.ddDN1QDL2gTN0czW}
    -use `cd /usr/share/doc/fontconfig` to change directory
    - `/challenge/run` prints the flag
5) pwn.college{wChFvNQUkGnH4ARYh7VsafziKPd.dhDN1QDL2gTN0czW}
    - `cd /etc`
    - `/challenge/run` prints the flag. 
6) pwn.college{w1yCMPg8-V4OTrwDjVLY0W13Ha6.dlDN1QDL2gTN0czW}
    - ` cd / ` to change to root, 
    - ` challenge/run ` to run the file from a relative path giving out the flags. 
7) pwn.college{UyPnQu8u0SakpG5nwBzJCnPBSv9.dBTN1QDL2gTN0czW}
    - `cd /` to change to root directory
    - we have to use . to run the relative file 
    - ` ./challenge/run` prints the flag. 
8) pwn.college{InBNd5IWwAiLOCojvXYRuhtsItU.dFTN1QDL2gTN0czW}
    -`cd /challenge`
    - we need to run 'run' in the same directory
    - `./run` prints the flag. 
9) pwn.college{cqA5M9iQWgzNor2GidlQ8AB8An0.dNzM4QDL2gTN0czW}
    -use ' ~/' to refrence home directory,
    - `/challenge/run ~/c` prints the flag. 

