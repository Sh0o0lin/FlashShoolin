# <span style="color:#4392F1">Unix/Linux Flash</span>


## <span style="color:#D8E5B"> File Commands </span>
- <span style="color:#D81E5B"> List directory </span>

        ls 

    ### <span style="color:#7EB77F">Output</span>
    
    ```
    PythonFlash.md  README.md  UnixFlash.md
    ``` 


- <span style="color:#D81E5B"> Formatted listing with hidden files </span>

        ls -al

    ### <span style="color:#7EB77F">Output</span>
    
    ```
    total 124
    drwxrwxr-x  2 mr_nimbus mr_nimbus   4096 Oct  2 14:08 .
    drwxr-xr-x 46 mr_nimbus mr_nimbus   4096 Oct  2 14:07 ..
    -rw-rw-r--  1 mr_nimbus mr_nimbus 112847 Oct  2 13:37 PythonFlash.md
    -rw-rw-r--  1 mr_nimbus mr_nimbus      0 Oct  2 14:08 README.md
    -rw-rw-r--  1 mr_nimbus mr_nimbus   1049 Oct  2 14:04 UnixFlash.md
    ```

- <span style="color:#D81E5B"> Force remove directory </span>

        rm -rf dir 

    ### <span style="color:#7EB77F">Output</span>
    
    ```
    dir and its files will deleted (-r delete dir, -f delete files)
    ```     

- <span style="color:#D81E5B"> Copy content </span>

        cp -r dir1 dir2 

    ### <span style="color:#7EB77F">Output</span>
    
    ```
    copy dir1 to dir2 (-r create dir2 if it doesn't exist)
    ```     
 
- <span style="color:#D81E5B"> Rename or Move file </span>

        mv file1 file2  

    ### <span style="color:#7EB77F">Output</span>
    
    ```
    will rename file1 to file2
    ```     

