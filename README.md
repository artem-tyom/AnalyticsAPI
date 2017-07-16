# Analytics API project description

## Project Overview 
Implement an Web service which provides an HTTP API for acessing some analytic metrics.   
### Objective
Import provided data into database and implement an web service which will calculate and send back some analytical metrics based on input arguments via some defined API.
### Technical Specifications
Implementation should be based on Layered Architecture. 
Application should have Presentation, Business and Data Access Layers.
#### 1. Database
Any relation database.

#### 2. Framework stack
Spring framework,
Struts2
  
#### 3. Api Protocol

##### 3.1 End Points
API should have following end-points
  1. DAU (Daily active users)  
  2. Retention                 
  
##### 3.1 API format
  API should be implemented according to REST format.
###### 3.2.1 DAU
Api accepts list of dates in dd/mm/yyyy format and returns DAU for that days.
###### 3.2.1 Retention
Api accepts two arguments. One is retention type. Accepted values are : "Day1", "Day7", "Day40".
The second one is date in dd/mm/yyyy format. Retention should be calculated starting from that day.
Returns the retention for that day.
