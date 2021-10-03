# Unix/Linux Flash


## File Commands
-  ### **List directory** 

        ls 

    #### **Output**
    
    ```
    PythonFlash.md  README.md  UnixFlash.md
    ``` 


- ### **Formatted listing with hidden files** 

        ls -al

    #### **Output**
    
    ```
    total 124
    drwxrwxr-x  2 mr_nimbus mr_nimbus   4096 Oct  2 14:08 .
    drwxr-xr-x 46 mr_nimbus mr_nimbus   4096 Oct  2 14:07 ..
    -rw-rw-r--  1 mr_nimbus mr_nimbus 112847 Oct  2 13:37 PythonFlash.md
    -rw-rw-r--  1 mr_nimbus mr_nimbus      0 Oct  2 14:08 README.md
    -rw-rw-r--  1 mr_nimbus mr_nimbus   1049 Oct  2 14:04 UnixFlash.md
    ```

- ### **Force remove directory** 

        rm -rf dir 

    #### **Output**
    
    ```
    dir and its files will deleted (-r delete dir, -f delete files)
    ```     

- ### **Copy content** 

        cp -r dir1 dir2 

    #### **Output**
    
    ```
    copy dir1 to dir2 (-r create dir2 if it doesn't exist)
    ```     
 
- ### **Rename or Move file** 

        mv file1 file2  

    #### **Output**
    
    ```
    will rename file1 to file2
    ```     

- ### **Create Symbolic Link lnk to file1**

        ln -s file1 lnk

    #### **Output**
    ```
    Address of file1
    ```
- ### **Create or Update file**

        touch file1

## AWK command 

- ### **Print File**

        awk '{print}' Test.txt

    #### **Output**
    ```
    ajay manager account 45000
    sunil clerk account 25000
    varun manager sales 50000
    amit manager account 47000
    tarun peon sales 15000
    deepak clerk sales 23000
    sunil peon sales 13000
    satvik director purchase 80000
    ```

- ### **Print the lines which match the given pattern**

        awk '/manager/ {print}' Test.txt

    #### **Output**
    ```
    ajay manager account 45000
    varun manager sales 50000
    amit manager account 47000
    ```

- ### **Splitting a Line Into Fields**

        awk '{print $1,$4}' Test.txt

    #### **Output**
    ```
    ajay 45000
    sunil 25000
    varun 50000
    amit 47000
    tarun 15000
    deepak 23000
    sunil 13000
    satvik 80000
    ```

- ### **Use of NR built-in variables (Display Line Number)**

        awk '{print NR,$0}' Test.txt
    
    #### **Output**
    ```
    1 ajay manager account 45000
    2 sunil clerk account 25000
    3 varun manager sales 50000
    4 amit manager account 47000
    5 tarun peon sales 15000
    6 deepak clerk sales 23000
    7 sunil peon sales 13000
    8 satvik director purchase 80000 
    ```

- ### **Use of NF built-in variables (Display Last Field)**

        awk '{print $1,$NF}' Test.txt

    #### **Output**
    ```
    ajay 45000
    sunil 25000
    varun 50000
    amit 47000
    tarun 15000
    deepak 23000
    sunil 13000
    satvik 80000
    ```

- ### **Another use of NR built-in variables (Display Line From 3 to 6)**

        awk 'NR==3, NR==6 {print NR,$0}' Test.txt

    #### **Output**
    ```
    3 varun manager sales 50000
    4 amit manager account 47000
    5 tarun peon sales 15000
    6 deepak clerk sales 23000
    ```

- ### **Format output**

        awk '{print NR "- " $1 }' Test.txt

    #### **Output**
    ```
    1- ajay
    2- sunil
    3- varun
    4- amit
    5- tarun
    6- deepak
    7- sunil
    8- satvik
    ```
