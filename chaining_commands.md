# Chaining Commands

### Flags and writeups

1) pwn.college{YdhBzLWITIqETMMtPb5htGjUcz8.dVTN4QDL2gTN0czW}
    - ; is used to write multiple commands in the same line
    -`/challenge/pwn; /challenge/college` prints the flag. 
2) pwn.college{A3Gxy6pARxcu6CAzgHUMQ0wBCQM.dFzN4QDL2gTN0czW}
    - use nano to create a bash script x.sh, 
    - `bash x.sh` to run the shell script giving us the flag
3) pwn.college{oRsfL_OnQA5DE9QJUMu-nCbStNB.dhTM5QDL2gTN0czW}
    - Use the same script from previous problem but just pipe the output to '/challenge/solve'
    - `bash x.sh | /challenge/solve` will give the flag. 
4) pwn.college{gsSeYgoLg9noLtGzRKKgJZWsDrK.dRzNyUDL2gTN0czW}
    - create script to invoke .sh script invoking /challenge/solve
    - `chmod +x ./uwu.sh`changing perms
    - `./uwu.sh` prints the flag. 

