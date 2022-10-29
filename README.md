## Repository of data and script used by the article: **Methodological proposal to identify the nationality of Twitter users through Random-Forests**

We have saved 30 tables in two repositories: repository 1 and repository 2.   
**Repository 1** has 12 tables:  https://github.com/damian-quijano/identify_nationality_twitter    
http://dx.doi.org/10.5281/zenodo.7254532     
**Repository 2** has 18 tables: https://github.com/damian-quijano/-identify_nationality_twitter2   
http://dx.doi.org/10.5281/zenodo.7254534     
   
Large tables have been saved in the first repository, small size tables and code have been saved in the second repository.  
  
**This is repository 1**. Below are the names and sizes of the largest tables used in the study.It is a group of 12 tables.


| Sequence 	| Table           	| File txt        	| Records 	| Size kb txt 	| Size kb zip 	|
|----------	|-----------------	|-----------------	|---------	|-------------	|-------------	|
| 1        	| DataTweetsCR_D1 	| DataTweetsCR_D1 	| 727169  	| 233553      	|             	|
| 1        	| DataTweetsGT_D1 	| DataTweetsGT_D1 	| 917048  	| 286160      	|             	|
| 1        	| DataTweetsHN_D1 	| DataTweetsHN_D1 	| 547655  	| 174158      	|             	|
| 1        	| DataTweetsNI_D1 	| DataTweetsNI_D1 	| 380458  	| 124279      	|             	|
| 1        	| DataTweetsPA_D1 	| DataTweetsPA_D1 	| 1236261 	| 419665      	|             	|
| 1        	| DataTweetsSV_D1 	| DataTweetsSV_D1 	| 591711  	| 212904      	|             	|
| 3        	| DataTweetsCR_D2 	| DataTweetsCR_D2 	| 2551889 	| 873283      	| 238156      	|
| 3        	| DataTweetsNI_D2 	| DataTweetsNI_D2 	| 1272375 	| 487276      	| 123409      	|
| 3        	| DataTweetsPA_D2 	| DataTweetsPA_D2 	| 4657755 	| 1692831     	| 459160      	|
| 6        	| resultsCR       	| resultsCR       	| 196420  	| 100446      	|             	|
| 6        	| resultsNI       	| resultsNI       	| 196420  	| 100513      	|             	|
| 6        	| resultsPA       	| resultsPA       	| 196420  	| 100493      	|             	|

**Sequence** refers to the order in which data is generated from the above tables. This means that if the table has sequence 3 it was created from the data in the table with sequence 2.  
In this repository the tables with sequence 1,3 and 6 are stored. In repository 2 are the tables with sequences 2,4,5,7 and 8.  
Size kb txt means that the file size is in kilobytes and text format. Size kb zip it means the same but in compressed format.  
   
*Below is shown data structure of the following tables*: **DataTweetsCR_D1,DataTweetsGT_D1,DataTweetsHN_D1,DataTweetsNI_D1, DataTweetsPA_D1, DataTweetsSV_D1, DataTweetsCR_D2, DataTweetsNI_D2 and DataTweetsPA_D2**  
| Field               	| Type         	| Description                       	|
|---------------------	|--------------	|-----------------------------------	|
| idt                 	| bigint       	| id tweet                          	|
| author_id           	| bigint       	| author                            	|
| text                	| varchar(MAX) 	| message                           	|
| created_at          	| varchar(50)  	|                                   	|
| source              	| varchar(50)  	| device                            	|
| conversation_id     	| bigint       	| id conversation thread            	|
| retweet_count       	| int          	|                                   	|
| reply_count         	| int          	|                                   	|
| like_count          	| int          	|                                   	|
| quote_count         	| int          	|                                   	|
| [user]              	| varchar(MAX) 	|                                   	|
| username            	| varchar(50)  	|                                   	|
| verified            	| varchar(50)  	|                                   	|
| in_reply_to_user_id 	| varchar(50)  	| to which user replied the message 	|
| referenced_tweets   	| varchar(MAX) 	| users you referred                	|
| hashtags            	| varchar(MAX) 	|                                   	|
| mentions            	| varchar(MAX) 	| users you mentioned               	|
  
  
*Data structure of the following tables:*  **resultsCR, resultsNI and resultsPA** .  
| Field  	| Type         	| Description                             	|
|--------	|--------------	|-----------------------------------------	|
| num    	| int          	| consecutive number                      	|
| pais   	| varchar(50)  	| country                                 	|
| TN     	| int          	| True Negative                           	|
| FP     	| int          	| False Positive                          	|
| FN     	| int          	| False Negative                          	|
| TP     	| int          	| True Positive                           	|
| cols   	| varchar(MAX) 	| unused columns or features              	|
| split  	| varchar(MAX) 	| test_size=0.20,      random_state = 123 	|
| params 	| varchar(MAX) 	| parameters used in the model            	|
| grid   	| varchar(MAX) 	| parameters used by GridSearch           	|
| best   	| varchar(MAX) 	| best parameters                         	|
  


