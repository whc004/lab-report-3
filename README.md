# grep
## grep -l
 ```
[cs15lwi23agm@ieng6-202]:berlitz2:307$ grep -l "Lucayans" Bahamas-History.txt 
Bahamas-History.txt
```
We can find a file that contain a single string which is very useful when we want to find a specific word(Lucayans here). If we have an specific word that is very uncommon, we can definitely use this command to help us.
```
[cs15lwi23agm@ieng6-202]:berlitz2:306$ grep -l "1000" Boston-WhereToGo.txt
Boston-WhereToGo.txt
```
When we have a lot of data, we can find which files contain that single number(1000 here), which is like an search engine and search for the content inside the file.

## git grep -c 

```
[cs15lwi23agm@ieng6-202]:berlitz2:309$ grep -c "china" Bermuda-WhatToDo.txt 
2
```
We can find a file that shows how many specific word it have(it search for china here). It could be useful when we want to find a single word or a word that contain this specific word.
```
[cs15lwi23agm@ieng6-202]:berlitz2:310$ grep -c "1000" Portugal-WhatToDo.txt
1
```
It totally work we want to check do we mention any data too many time in a file and save a lot of time(it search for 1000 here). 
## git grep -n

```
[cs15lwi23agm@ieng6-202]:berlitz2:311$ grep -n "china" Bermuda-WhatToDo.txt
57:The oldest department store is Trimingham’s, which has a comprehensive range of designer goods such as perfume and clothing, but other stores act as exclusive agents for certain producers (for example, Bluck’s and Cooper’s specialize in china and crystal). 
70:The military and colonial legacy of Bermuda, plus a natural tendency for most Bermudian families in the past never to throw anything away, means that the island is a treasure trove of collectibles. Many items found their way over from Britain, so old tins, buttons, bottles, and items of china and brass are numerous. You’ll find small stalls and shops in the alleys of Hamilton and on the roadside as you travel around the island where you can lose yourself for hours searching for that little piece of the past to take home with you.
```
This command return the file-name, line, and the content of the line, which is like a dictionary. Here we search "china" it appear a lot of content have china and the word contain china.
```[cs15lwi23agm@ieng6-202]:berlitz2:311$ grep -n "china" Bermuda-WhatToDo.txt
57:The oldest department store is Trimingham’s, which has a comprehensive range of designer goods such as perfume and clothing, but other stores act as exclusive agents for certain producers (for example, Bluck’s and Cooper’s specialize in china and crystal). 
70:The military and colonial legacy of Bermuda, plus a natural tendency for most Bermudian families in the past never to throw anything away, means that the island is a treasure trove of collectibles. Many items found their way over from Britain, so old tins, buttons, bottles, and items of china and brass are numerous. You’ll find small stalls and shops in the alleys of Hamilton and on the roadside as you travel around the island where you can lose yourself for hours searching for that little piece of the past to take home with you.
[cs15lwi23agm@ieng6-202]:berlitz2:312$ grep -n "1000" Portugal-WhatToDo.txt
34:Fishing. All along the coast you will see anglers in boots casting off from the beaches, and others perched on rocks or man-made promontories. A permit is needed for river and lake fishing; details are available from branches of the Portuguese National Tourist Office (see page 169) or the Instituto Florestal (Avenida João Crisóstomo 26, 1000 Lisbon). Angling conditions are generally best in the winter from October to mid-January.
```
This command shows the search result of chinatown instead of china which is more accurate if we find this word.
## git grep -e
```
[cs15lwi23agm@ieng6-202]:berlitz1:328$ grep -e "chinatown" -e "heartland" WhereToMalaysia.txt
        Chinatown. The heartland of Georgetown’s chinatown is
```
This command shows the file name and the content of two string "chinatown" and "heartland" in the same line.
```
[cs15lwi23agm@ieng6-202]:berlitz2:314$ grep -e "china" -e heartland Bermuda-WhereToGo.txt
Just behind the Post Office is a building that houses the Bermuda National Library and the Historical Society Museum, prime collections devoted to important historical documents and artifacts from the island. The public rooms are small but full of Bermudian treasures. Silver, china, coins, and furniture have been gathered together, including rare and valuable “hog” money as well as some of the Confederate notes that were used to pay for goods before the Civil War. Many Bermudian businessmen and sailors were paid in money that became worthless after the Unionists won the war.
Set in the far northeast portion of Bermuda, St. George’s is the island’s oldest town and the historic heartland of the colony. Sir George Somers and his brave band of settlers were heading for Virginia in 1609 when they were shipwrecked on reefs just offshore from here. They were surprised by the natural riches that Bermuda had to offer, as the island had good cedar wood to build more ships. Out of adversity came good fortune, and the settlers soon built two new ships and sailed from Bermuda to complete their original goal of reaching Jamestown. Somers returned to Bermuda the following year but died here before he could develop the town further.
```
This command shows the file name and the content of two string "china" and "heartland" which do not need to in the same line.


### Source
I find this website when I search "grep command"
https://www.geeksforgeeks.org/grep-command-in-unixlinux/
