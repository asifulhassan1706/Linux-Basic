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
