# Unix/Linux Flash


## File Commands
-  List directory 

        ls 

    ### Output
    
    ```
    PythonFlash.md  README.md  UnixFlash.md
    ``` 


-  Formatted listing with hidden files 

        ls -al

    ### Output
    
    ```
    total 124
    drwxrwxr-x  2 mr_nimbus mr_nimbus   4096 Oct  2 14:08 .
    drwxr-xr-x 46 mr_nimbus mr_nimbus   4096 Oct  2 14:07 ..
    -rw-rw-r--  1 mr_nimbus mr_nimbus 112847 Oct  2 13:37 PythonFlash.md
    -rw-rw-r--  1 mr_nimbus mr_nimbus      0 Oct  2 14:08 README.md
    -rw-rw-r--  1 mr_nimbus mr_nimbus   1049 Oct  2 14:04 UnixFlash.md
    ```

-  Force remove directory 

        rm -rf dir 

    ### Output
    
    ```
    dir and its files will deleted (-r delete dir, -f delete files)
    ```     

-  Copy content 

        cp -r dir1 dir2 

    ### Output
    
    ```
    copy dir1 to dir2 (-r create dir2 if it doesn't exist)
    ```     
 
-  Rename or Move file 

        mv file1 file2  

    ### Output
    
    ```
    will rename file1 to file2
    ```     
