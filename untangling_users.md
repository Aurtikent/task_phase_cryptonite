1) pwn.college{InyNZu5pZRJI1DuBM4OxuU1_qqu.dVTN0UDL2gTN0czW}
    -`su` is used to spawn a root shell when checked with the root password (obeselete)
    - to get the flag run `su` 
    - use password `hack-the-planet`
    - `cat /flag` to get the flag. 
2)pwn.college{oeZo94RvaR6ekBzB0CKKVXoKmzv.dZTN0UDL2gTN0czW}
    - become user zarus with `su zardus` with the given password 'dont-hack-me'
    - `/challenge/run` will give you the fla.g
3) pwn.college{0LJC9enMSBoCn2cFilprIhBisBp.ddTN0UDL2gTN0czW}
    - we need use JohntheRipper to crack the leaked shadow file given to us. 
    - run `john /challenge/shadow-leak` this process will run for some time cracking the password, 
    - use the <password> with `su zardus`
    - now run `/challenge/run` which will give you the flag. 
4) pwn.college{E4s0ZStcxSC7sJaMj_T-cCu1aGG.dhTN0UDL2gTN0czW}
    - sudo is mordern replacement for su, for security purposes. 
    - `sudo cat flag` will give the flag. 

