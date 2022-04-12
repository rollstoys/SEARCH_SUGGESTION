# Search Suggestions

Api to retrieve the list of counties and states based on the fragment of the word.

## Getting Started

This is developed using spring-boot and the database used is H2 Db, The data is initially loaded into the DB on application startup

### Dependencies

* Java 9 and above

### Executing program

* Extract the contents of the compressed file , and open cmd prompt on the jar directory.
* Execute the below command in the prompt.
```
java -jar FS_SEARCH-0.0.1-SNAPSHOT
```

### EndPoint

GET /suggest

|parameter type 	   |name | type	|
|------------------	   |-----|------|
|query  param   	   | q	 | String|


### Request sample
```
GET localhost:3000/suggest?q=wa
```

### Sample response
```
status:200
responsebody:
[{"FIPS":53001,"STATE":"WA","NAME":"Adams"},{"FIPS":53003,"STATE":"WA","NAME":"Asotin"},{"FIPS":53005,"STATE":"WA","NAME":"Benton"},{"FIPS":53007,"STATE":"WA","NAME":"Chelan"},{"FIPS":53009,"STATE":"WA","NAME":"Clallam"}]
```





