# Shell-data-processing

## Project:

- In the already existing folder 44517 which is my Big-Data course number, I have created a new subfolder called shell-data-processing with the help of the command: ``` mkdir shell-data-processing ```
- I have added two items README.md and .gitignore with the help of command : ```ni README.MD``` and ```ni .gitignore```.
- For listing the items in the list we use this command : ``` ls ```

## Curl 

- As any particular topic is not mandatory, I have chosen topic of my all time interest which is Cricket ball. I went to cricket ball in wikipedia and copied the url there which is "https://en.wikipedia.org/wiki/Cricket_ball".
- Next step was to return the page text with the help of curl command : 
``` curl "https://en.wikipedia.org/wiki/Cricket_ball" ``` 
- Then i had to return the page text and copied the output to the file with the help of curl command :
``` curl "https://en.wikipedia.org/wiki/Cricket_ball" -0 data.txt ```
- Now to get out of the powershell, we use a command :
``` exit ```

## Bash  
 - Now we'll use some Bash commands to process the text
 - For transforming each space into a return character we use :
 ``` tr ' ' '\12' < data.txt ```
 - To send the output of one command as an input of another command we use :
 ``` tr ' ' '\12' < data.txt | sort ```
 - We sort based on the count using :
 ``` tr ' ' '\12' < data.txt | sort | uniq -c ```
 - To pipe the reduced output to sort with the help of -nr flag, we use :
 ``` tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr ```
 - To redirect the result to result.txt we use :
 ``` tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt ```
 
 
 - The  Bash up arrow ``` ^ ``` brings the previously used command in the bash shell.
 - ``` sort --help ``` is used to list all the functional parameters which can be used along with sort command .
 - ``` -n ``` command used for numeric sort to compare according to string numerical value.
 - ``` -r ``` used for reversing the result of comparisions according to the word.
 - There is one dash for a single letter flag.for example: ``` -R ```
 - There are two dashes when the flag is more than one letter. for Example: ``` --version-sort  ```
 - ``` cat ``` command is used to show the content of a document,append and also creating a document.
 
 - ![Bash Commands](https://github.com/manideepchamala/shell-data-processing-/blob/master/Screenshot%20(66).png)
 
 
 


