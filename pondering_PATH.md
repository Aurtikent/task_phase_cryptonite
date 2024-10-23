# Pondering PATH

### Flags and Writeups, 

1) pwn.college{AoeRX2FxY4vGzGrdNC2IQzNYLE5.dZzNwUDL2gTN0czW}
    - messing with the PATH variable to so that the 'run' binary cannot find the ls command
    - `PATH=''` this will empty the PATH VARIABLE
    - now running `/challenege/run` will give the flag. 
2) pwn.college{8SywImjzvCffpuZlAAmOy6bFzhl.dVzNyUDL2gTN0czW}
    - `PATH=/challenge/more_commands/`
    - `/challenge/run` will give the flag,
3) pwn.college{gOSk0hl01jH12Vy_q6F4_CAVkJ8.dZzNyUDL2gTN0czW}
    - create a shell script named `win`, and add `cat /flag` to it.
    - now do `export PATH="/home/hacker:$PATH"` this will add your home directory to path 
    - now `/challenge/run` will give you the flag. 
4) pwn.college{0zYeW_Z4p5dijWPpSCJ-6xVCPNO.ddzNyUDL2gTN0czW}
    - We have to modify path for this challenge, 
    - PATH works sequentially ie it looks for the commands one after the other in the directory and uses the first instance it finds. 
    - we create a script called `rm` with `cat /flag` in it. 
    - make it executable with `chmod +x ./rm`
    - add your home dir to path in the front with `PATH="/home/hacker:$PATH"`
    - run `/challenge/run` it will print the flag. 
    
