# Practicing Piping 

## Notes and Flags. 

1) pwn.college{cb4ugUAVmNZRLCPwpOqAK0EcquF.dRjN1QDL2gTN0czW}
    - `echo PWN > COLLEGE` 

2) pwn.college{MQTR8wTY_GEB3LAPseFA7a5gAHg.dVjN1QDL2gTN0czW}
    - challenge asked us to redirect output of '/challenge/run' to a file called 'myflag' to print the flag.
    - `/challenge/run > myflag` gets us the flag in the file 'myflag'
    - `cat myflag` will print the flag to the terminal. 

3) pwn.college{M0utH9uvRzd-J8YtJM6dK-0UXwQ.ddDM5QDL2gTN0czW}
    - `>>` appends to the specified file instead of overwriting it like `>` does. 
    - The run binary prints half the flag to stdout and appends half the flag to the 'the-flag' file,
    - To get the complete flag run: `/challenge/run >> the-flag`

4) pwn.college{Mnx-LXcuzub3j4-WcjEDNvoP93d.ddjN1QDL2gTN0czW}
    - The challenge is on redirecting file descriptors,     
    - `/challenge/run 1> myflag 2> instructions` will print the flag to 'myflag' and the diagnostics to 'instructions'
    - if the command was run correctly, `cat myflag` will give the flag. 
5) pwn.college{kv97yHPWX9PkfnHlh96wVEN5CsR.dBzN1QDL2gTN0czW}
    - Gotta Use Redirecting stdinput,
    - `echo COLLEGE > PWN` to create the file "PWN" with "COLLEGE" in it
    - redirecting input `/challenge/run < PWN` will print the flag. 

6) pwn.college{ULozDiREs6VzGphqdyrg4F-3wyP.dhTM4QDL2gTN0czW}
    - Gotta use grep and file descriptor to solve the challenge
    - `/challenge/run > /tmp/data.txt` as prescribed the by the description
    - flag contains 'pwn.college' so grepping for the same will print the flag, 
    - `cat /tmp/data.txt | grep pwn.college` prints the flag. 
7) pwn.college{w0XOCJSVdEeqBvMTdeO4cxeh586.dlTM4QDL2gTN0czW}
    -using the ' | ' operator to pipe the output from stdout of command to stdin of another command.
    -`/challenge/run | grep pwn.college` will print the flag to the terminal. 

8) pwn.college{kCrU0_zYehuMqgppcs0_gTC8pz1.dVDM5QDL2gTN0czW}
    - The shell has a >& operator, which redirects a file descriptor to another file descriptor.
    - We can use this to direct the stderr to stdout and then pipe that to grep,
    - `/challenge/run 2>&1 | grep pwn.colle` will print the flag. 

9) pwn.college{gNcP6o6-Yn2OYQJZTrZ6gwqakYK.dFjM5QDL2gTN0czW}
    - `tee` acts like a T-pipe in plumbing it copies the stdin to stdout and files prescribed to it. 
    - `/challenge/pwn | tee out.txt | /challenge/college` in the challenge we use tee to check what is the problem 'pwn' binary 
    - `cat out.txt` tells us that SECRET_ARG should be "gNcP6o6-" with a --secret argument to 'pwn'.
    -  `/challenge/pwn --secret gNcP6o6- | /challenge/college` prints the flag to the terminal. 

10) pwn.college{c9YS1ePc3YPVMQboWmY8uVTk0gR.dBDO0UDL2gTN0czW}
    - `/challenge/hack | tee >(/challenge/the) >(/challenge/planet)` will print the flag.
    - we need to 'process substitute' both the commands and pass the outputs of `/challenge/hack` to both 'the','planet' programs at the same time. 

11) pwn.college{wUXyMMlSv4R5Jdgc1kOWz0UBUV3.dFDNwYDL2gTN0czW}
    - complex appearing problem which in practice is indeed easy.
    - `/challenge/hack 2> >(/challenge/the) 1> >(/challenge/planet)` will give you the flag,
    - redirecting the stdout to different program, and redirecting the stdin to different program, nothing too complicated. 


 
    
