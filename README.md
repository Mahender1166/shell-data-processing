# Shell data processing commands
## Curl commands used
- ```curl "url"``` (url is the webiste url) is the command unsed to get the data from the URL. Note: The url is used id https://en.wikipedia.org/wiki/Pablo_Picasso.
- ```curl "url" -O data.txt``` this command is used to store the obtained data into a text file named data.
<br>
We can performa any operation required on this data.txt file as per our requirement.

## Text processing commands 
- To transform '' into a return character '/12' we use ```tr ' ' '/12' < data.txt``` command.
- To sort the order we append ```|sort``` to the above command that is ```tr ' ' '/12' < data.txt | sort```
- To sort with unique character we use ```tr ' ' '/12' < data.txt | sort | uniq -c``` command.
- To sort the data with numeric and reverse order we can use this command ```tr ' ' '/12' < data.txt | sort | uniq -c | sort -nr``` where ```-n``` stands for neumaric and ```-r``` stands for reverse order.
- To store result into a text file we use ```< fileName.txt``` at the end of the command. For example, we if we want to store result of the above data command we can write as follows : ```tr ' ' '/12' < data.txt | sort | uniq -c | sort -nr <result.txt```
- If we use single aplhabet to represent any command we use single dash infront of it and two dashes when we have a command with more than one alphabet. For example ```-r``` and ```--reverse``` if we want to write whole word. But both works the same they sort the data in reverse order.
- We can get the command which we have executed before by clicking the upwards arrow key from the keyboard. 

## Bash commands
- we can use ```<``` command for inserting the data into a text file.
- we can use ```<<``` command for appending the new data at the end of the file.
- we can use ```cat``` command to display the contents of the file.
- we can use ```ls``` command to display the files in that directory.