## 1. Build the network diagram

---

### About the data
The data describes the reading behaviour of Manning Publications' liveBook platform users. It contains 4999 observations, each defined by nine features. 

| Feature                 	| Definition                                                     	|
|:------------------------	|:---------------------------------------------------------------	|
| `user_id`               	| User's unique identification                                   	|
| `number_of_ticks`       	| Number of server ticks (30 seconds each) a user spends reading 	|
| `date_created`          	| Date and time the user started to read                         	|
| `chapter`               	| Chapter of `book` being read                                   	|
| `book`                  	| Book being read                                                	|
| `numberofentriesofbook` 	| Number of referenced points of the book                        	|
| `numberofusersofbook`   	| Number of users who read the book                              	|
| `product_manning_id`    	| Book's unique identification                                   	|
| `user_owns_book`        	| Whether the user purchased the book                            	|

### Theory
A network diagram will be implemented, allowing us to examine the relationships between Manning Pubilcations' (Manning) customers and Manning's books. Per graph theory, the nodes refer to Manning's books and the edges, the order in which their customers read them.

### Plan

1. Extract edge list from data with each edge defined as (source, target)
2. Build network diagram
3. Visualize network diagram for quality assurance
