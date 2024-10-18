# Shell Varibles, 

### Writeups and Flags. 

1) pwn.college{48eJduSH0AhGz3IAynVnw9gR69p.ddTN1QDL2gTN0czW}
    - `echo $FLAG` 
    - '$' refers to a shell varible, echo prints the command. 

2) pwn.college{UBq2OjYbvtzoswM4B1btWh0cW5G.dlTN1QDL2gTN0czW}
    - ` PWN=COLLEGE`
    - prints the flag. 
3) pwn.college{wLzQ82-XW6AIhr-3Q94czBXQF3s.dBjN1QDL2gTN0czW}
    - `PWN="COLLEGE YEAH"` 
    - needs quotes so shell does interprete it as a new command.
4) pwn.college{c5fD-P_rK83WNiR3kjQTRYwEqXr.dJjN1QDL2gTN0czW}
    - Need to export variables so that child processes see them,
    - for the challenge:
    - `PWN=COLLEGE`
    - `export PWN`
    - `COLLEGE=PWN`
    - `/challenge/run` will print the flag. 
5) pwn.college{sxZgyqfWyfTOHszay69DXwXV2Hp.dhTN1QDL2gTN0czW}
    - `env`  will print all the exported varibles of the shell, 
    - lot of data, hence `env | grep FLAG` gives us the flag. 
6) pwn.college{cICKxdQwZOGBXAOvZSUk_avEBLk.dVzN0UDL2gTN0czW}
    - `PWN=$(/challenge/run)`
    - `echo $PWN`
7) pwn.college{MiGqEBKwbk2tXB4GDV17fMcLSgC.dhzN1QDL2gTN0czW}
    - 'read'' will read input in terminal on stdin
    - `read PWN` and then enter input `"COLLEGE"` will print the flag. 
8) pwn.college{oa_NCeETqF7ztfXwPuulYLrILlc.dBjM4QDL2gTN0czW}
    - `read PWN < /challenge/read_me` 
    - give in to the stdin of Read which writes it to PWN.


