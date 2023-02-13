# grep
## git grep -l
 ```
[cs15lwi23agm@ieng6-201]:skill-demo1-data:211$ git grep -l Lucayans
written_2/travel_guides/berlitz2/Bahamas-History.txt 
```
We can find a file that contain a single string which is very useful when we want to find a specific word(Lucayans here). If we have an specific word that is very uncommon, we can definitely use this command to help us.
```
[cs15lwi23agm@ieng6-201]:skill-demo1-data:213$ git grep -l 1000
written_2/travel_guides/berlitz1/HistoryIsrael.txt
written_2/travel_guides/berlitz1/HistoryIstanbul.txt
written_2/travel_guides/berlitz1/HistoryItaly.txt
written_2/travel_guides/berlitz1/HistoryJamaica.txt
written_2/travel_guides/berlitz1/HistoryJerusalem.txt
written_2/travel_guides/berlitz1/IntroLasVegas.txt
written_2/travel_guides/berlitz1/WhereToIndia.txt
written_2/travel_guides/berlitz1/WhereToIstanbul.txt
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt
written_2/travel_guides/berlitz2/Bali-History.txt
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
written_2/travel_guides/berlitz2/Budapest-History.txt
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
written_2/travel_guides/berlitz2/Canada-History.txt
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt
written_2/travel_guides/berlitz2/Cuba-History.txt
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt
written_2/travel_guides/berlitz2/Vallarta-History.txt
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt
```
When we have a lot of data, we can find which files contain that single number(1000 here), which is like an search engine and search for the content inside the file.

## git grep -c 

```
[cs15lwi23agm@ieng6-201]:skill-demo1-data:224$ git grep -c china
written_2/non-fiction/OUP/Abernathy/ch2.txt:1
written_2/travel_guides/berlitz1/HistoryFrance.txt:2
written_2/travel_guides/berlitz1/HistoryJapan.txt:2
written_2/travel_guides/berlitz1/HistoryMalaysia.txt:2
written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:1
written_2/travel_guides/berlitz1/WhatToHongKong.txt:2
written_2/travel_guides/berlitz1/WhereToFrance.txt:2
written_2/travel_guides/berlitz1/WhereToJapan.txt:3
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:1
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:3
written_2/travel_guides/berlitz2/Athens-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:1
written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt:1
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:1
written_2/travel_guides/berlitz2/Paris-WhatToDo.txt:1
```
We can find a file that shows how many specific word it have(it search for china here). It could be useful when we want to find a single word or a word that contain this specific word.
```
[cs15lwi23agm@ieng6-201]:skill-demo1-data:220$ git grep -c 1000
written_2/travel_guides/berlitz1/HistoryIsrael.txt:1
written_2/travel_guides/berlitz1/HistoryIstanbul.txt:1
written_2/travel_guides/berlitz1/HistoryItaly.txt:1
written_2/travel_guides/berlitz1/HistoryJamaica.txt:1
written_2/travel_guides/berlitz1/HistoryJerusalem.txt:1
written_2/travel_guides/berlitz1/IntroLasVegas.txt:1
written_2/travel_guides/berlitz1/WhereToIndia.txt:3
written_2/travel_guides/berlitz1/WhereToIstanbul.txt:1
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:1
written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:1
written_2/travel_guides/berlitz2/Bali-History.txt:1
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:1
written_2/travel_guides/berlitz2/Budapest-History.txt:1
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:1
written_2/travel_guides/berlitz2/Canada-History.txt:1
written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt:1
written_2/travel_guides/berlitz2/Cuba-History.txt:1
written_2/travel_guides/berlitz2/Paris-WhereToGo.txt:1
written_2/travel_guides/berlitz2/Portugal-WhatToDo.txt:1
written_2/travel_guides/berlitz2/PuertoRico-WhatToDo.txt:2
written_2/travel_guides/berlitz2/Vallarta-History.txt:1
written_2/travel_guides/berlitz2/Vallarta-WhatToDo.txt:1
```
It totally work we want to check do we mention any data too many time in a file and save a lot of time(it search for 1000 here). 
## git grep -n

```
[cs15lwi23agm@ieng6-201]:skill-demo1-data:227$ git grep -n china    
written_2/non-fiction/OUP/Abernathy/ch2.txt:15:Until the emergence of mass retail, the wholesaler-jobber dominated the distribution of consumer dry goods to general stores: clothing, upholstered furnishings, hardware, drugs, tobacco, furniture, china, and glassware. Unlike traveling peddlers of the past, who carried everything with them, these salesmen could ride the rails into town with no more than a trunk of samples and catalogs. The new infrastructure created by the railroads and telegraph contributed to the growth of wholesale houses. Retailers no longer needed to carry such large inventories, the risk of losing shipments was reduced, and delivery was more certain on a specified schedule. Increased volume cut unit costs and enhanced cash flow, reducing credit needs. Moreover, these salesmen provided a flow of information to their headquarters on changing demand in -various local
ities as well as the credit ratings of local storekeepers and merchants.
written_2/travel_guides/berlitz1/HistoryFrance.txt:399:        empire in North and West Africa and Indochina. Rediscovered national
written_2/travel_guides/berlitz1/HistoryFrance.txt:503:        Indochina, and elsewhere began to move to France and alter the French
written_2/travel_guides/berlitz1/HistoryJapan.txt:473:        French Indochina after the defeat of France. The US responded to the
written_2/travel_guides/berlitz1/HistoryJapan.txt:474:        Japanese invasion of Indochina with a trade and fuel embargo, cutting
written_2/travel_guides/berlitz1/HistoryMalaysia.txt:35:        Mekong valley of Indochina. Their rulers introduced Buddhist and Hindu
written_2/travel_guides/berlitz1/HistoryMalaysia.txt:370:        by Marshal P<C3><A9>tain<E2><80><99>s French colonial officials in Indochina and backed
written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:329:        scones served on fine bone china.
written_2/travel_guides/berlitz1/WhatToHongKong.txt:121:        china, are geared to entertain and instruct visiting tourists; prices
written_2/travel_guides/berlitz1/WhatToHongKong.txt:127:        duty-free situation, good bargains may be found in European china,
written_2/travel_guides/berlitz1/WhereToFrance.txt:1974:        china from France and the rest of the world. For a collection of early
written_2/travel_guides/berlitz1/WhereToFrance.txt:3271:        pottery, china, stoneware, and porcelain, with as many as 12,000<E2><80><82>items
written_2/travel_guides/berlitz1/WhereToJapan.txt:1955:        Furuimachinami streets. The high-quality craftwork here<E2><80>  
<82><E2><80><94><E2><80><82>woodcarvings,
written_2/travel_guides/berlitz1/WhereToJapan.txt:1956:        lacquerware, and pottery<E2><80><82><E2><80><94><E2><80><82>is renowned throughout Japan. Furuimachinami
written_2/travel_guides/berlitz1/WhereToJapan.txt:2336:        old. Beyond Aoshima the picturesque, winding Nichinan coast alter
```
This command return the file-name, line, and the content of the line, which is like a dictionary. Here we search "china" it appear a lot of content have china and the word contain china.
```
[cs15lwi23agm@ieng6-201]:skill-demo1-data:222$ git grep -n 1000
[cs15lwi23agm@ieng6-201]:skill-demo1-data:226$ git grep -n chinatown
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:1000:        Chinatown. The heartland of Georgetown<E2><80><99>s chinatown is
```
This command shows the search result of chinatown instead of china which is more accurate if we find this word.
## git grep -n 
```
[cs15lwi23agm@ieng6-201]:skill-demo1-data:249$ git grep --all-match -e chinatown --and -e heartland
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        Chinatown. The heartland of Georgetown<E2><80><99>s chinatown is
```
This command shows the file name and the content of two string "chinatown" and "heartland" in the same line.
```
[cs15lwi23agm@ieng6-201]:skill-demo1-data:250$ git grep --all-match -e china -e heartland
written_2/travel_guides/berlitz1/WhereToJapan.txt:        time Kyoto thrived as Japan<E2><80><99>s cultural and creative heartland. But the
written_2/travel_guides/berlitz1/WhereToJapan.txt:        Furuimachinami streets. The high-quality craftwork here<E2><80><82>   
<E2><80><94><E2><80><82>woodcarvings,
written_2/travel_guides/berlitz1/WhereToJapan.txt:        lacquerware, and pottery<E2><80><82><E2><80><94><E2><80><82>is renowned throughout Japan. Furuimachinami
written_2/travel_guides/berlitz1/WhereToJapan.txt:        old. Beyond Aoshima the picturesque, winding Nichinan coast alternates
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        group of famous hotels in Southeast Asia and Indo-china. In the    
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        Chinatown. The heartland of Georgetown<E2><80><99>s chinatown is   
written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        influenced by the kingdom of Funan in Indochina some 2,000 years   
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:Just behind the Post Office is a building that houses the Bermuda National Library and the Historical Society Museum, prime collections devoted to important historical documents and artifacts from the island. The public rooms are small but full of Bermudian treasures. Silver, china, coins, and furniture have been gathered together, including rare and valuable <E2><80><9C>hog<E2><80><9D> money as well as some of the Confederate notes that were used to pay for goods before the Civil War. Many Bermudian businessmen and sailors were paid in money that became worthless after the Unionists won the war.
written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:Set in the far northeast portion of Bermuda, St. George<E2><80><99>s is the island<E2><80><99>s oldest town and the historic heartland of the colony. Sir George Somers and his brave band of settlers were heading for Virginia in 1609 when they were shipwrecked on reefs just offshore from here. They were surprised by the natural riches that Bermuda had to offer, as the island had good cedar wood to build more ships. Out of adversity came good fortune, and the settlers soon built two new ships and sailed from Bermuda to complete their original goal of reaching Jamestown. Somers returned to Bermuda the following year but died here before he could develop the town further.
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:Harbourfront is a bright new neighborhood reclaimed from a swampy wasteland, at the foot of the CN Tower. Rundown warehouses and factories have been transformed into art galleries, bars, restaurants, boutiques, a sailing school, playgrounds in the park, and, more recently, chic apartments. Young upwardly mobile peddlers of old and new-old china and other bric-a-brac on Queen<E2><80><99>s Quay West call their flea market the Harbourfront Antique Market. The Canadian Railway Museum at Spadina Pier exhibits some of the earliest engines to cross the continent. For a thorough view of the port facilities, take the harbor boat tour organized by the Toronto Harbor Commission.
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:The 90-minute drive from Toronto to Niagara Falls (130 km/81 miles south of Toronto) curves around the west end of Lake Ontario through the province<E2><80><99>s industrial heartland<C2><A0><E2><80><94><C2><A0>Mississauga, Hamilton, and St. Catharines, known as the Golden Horseshoe. If you want to see the Falls without getting entangled overnight in the mob scene of the tourists (12 million visitors annually), stay over in the quieter town of Niagara-on-
```
This command shows the file name and the content of two string "china" and "heartland" which do not need to in the same line.
