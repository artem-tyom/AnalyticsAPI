# Analytics API project description

## Project Overview 

  Implement an Web service providing an API for accessing daily active users (DAU) and other analytic metrics. 
  
### Objective
Import provided data into database and implement an web service which will calculate and send DAU via some defined API.
### Technical Specifications
Implementation should be based on Layered Architecture. 
Application should have Presentation, Business and Data Access Layers.
#### 1. Database

  Any relation database.

#### 2. Framework stack

Spring framework,
Struts2
  
#### 3. Api Protocol

At this moment Api consists from single end-point giving access to DAU based on input arguments. 

  I.e  https://analytics-api.com/api?command=dau&args={INPUT_ARGS}


INPUT_ARGS is JSON object.


```javascript
//INPUT
{
app_id : some_unique_id,
dateFrom : 10/01/2017  //start date in  dd/mm/yyyy format,
dateTo : 10/02/2017
}
//OUTPUT
{
date1 : 212312, //DAU1
date2 : 645754, //DAU2
…
dateN : 96796 //DAUn
}

//Where  dateFrom <= N <= dateTo
```
