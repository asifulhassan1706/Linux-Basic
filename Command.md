### Commands

- ```pwd```: present working directory

- ```ls```: list directory

- ```cd```: change directory

- ```cd /```: take you to the root directory

- ```cd ~```: take you to the user home directory

- ```cd ./another_folder```: navigate from current directory to another_folder

- ```cd ..```: navigate from current directory to parent directory

- ```cd -```: go back to the previous working directory
  - ```cd /```: going to the root directory
  - ```cd ~/```: going to the home directory
  - ```cd -```: going back to the root directory


- ```cd "my work"``` or ```cd 'my work'``` or ```cd my\ work```: going to a folder with space

- ```ls /```: display your root directory

- ```ls ~```: display your home directory

- ```ls ..```: display the content of my parent directory

## LS Options

- ```ls```: List files by alphabetic order

- ```ls -i```: This will list the index node number of each file

- ```ls -a```: This will show all the files (-a == all files) in your current directory, including hidden files

- ```ls -l```: Long listing of all files in the directory and some important information.

- ```ls -t```: Sort files by modification date

- ```ls -r```: List the files in reverse fashion (in this case reverse based on alphabetic order)

- ```ls -rt OR ls -r -t```: List the file in reverse fashion (in this case reverse based on modification date)

- ```ls -li```: Long listing + show inode ids

- ```ls -lia```: Long listing + show inode ids + hidden files

- ```ls -R```: Show current directory content plus any children/sub directory content as well

## Touch Command (Create a file)

- Touch is used to create empty files

  - ```touch file_name```: Create a file called file_name
  - ```touch file_name1 file_name2 file_name3```: Creates 3 files
  - ```touch 'my file'``` or ```touch "my file"``` or ```touch my\ \ file```: create a file with a name containing spaces
    - ```\``` is a scape sequence


- Touch is also used to update a current files timestamp (modification dade)

  - ```touch newFile```
  - ```echo "test" > newFile```
  - ```touch newFile```: this will update the file timestamp and keep the content


- ```ls -Ra```: Show current directory content plus any children/sub directory content as well + including hidden files
