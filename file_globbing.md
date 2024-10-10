# File Globbing 
## Notes and Flags

1) pwn.college{IEDSD1ppGyjPkL9ssp7VhiMG2_e.dFjM4QDL2gTN0czW}
    - `*` is the wild character and can be used to replace any file which matches the pattern.
    - for the challenge `/ch*` changes the directory to /challenge
    - wherein you can run `./run` to print the flag.

2) pwn.college{kYqSM2BUsCZNd3CcPTgg_OL8qWZ.dJjM4QDL2gTN0czW}
    - `?` is another wildcard character but it only replaces upto 1 character 
    - following the same principle, we use `cd /?ha??enge` to change the directory, and then `./run` to print the flag.

3) pwn.college{UfLiXorngET5-JYb2P9l6uBftwy.dNjM4QDL2gTN0czW}
    - `[]` is like a wild-card multiple choice ie the pattern matching will only occur with the characters which are inside the [].
    - following instructions, `cd /challenge/files` 
    - now as per challenge description we use `[]` to pass the arguments to /challenge/run ie `/challenge/run file_[shab]`, this gives us the flag. 

4) pwn.college{w9iQBjGJZVIjjoJdNNb3uYEkjNm.dRjM4QDL2gTN0czW}
    - `[]` can be used to expand on absolute file paths as well. 
    -   `/challenge/run /challenge/files/file_[absh]` gives us the flag. 

5) pwn.college{4syMFiU10XZ6fpUkHsndqThj1iA.dVjM4QDL2gTN0czW}

    - This was a tricky one, following description we `cd /challenge/files` and see the files.

[Photo of the files](images/globbing_file_names_5.png)

    - Interesting thing we notice is that there is only 1 filename with starting with each letter. 
    - so `[cep]*` would expand to the file names we need 
    - running  `/challenge/run [cep]*` gives us the flag. 

6) pwn.college{Yg-dr1jMD7yN14Mgkqm-PVKiYB4.dZjM4QDL2gTN0czW}
    - `[!<patter,letters>]` the "!" or "^"acts as an invert and disincludes the chars in the "[]"
    - Similar to Challenge 5, we notice only 1 filename per letter in the `/challenge/files` directory
    - `/challenge/run [!pwn]*` gives us the flag. 






