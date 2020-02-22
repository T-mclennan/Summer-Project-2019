# [Safe SF Hazard Reporting Platform](http://safesf.ddns.net/)

---

#### This project was from the summer semester of 2019 Software Design class. We worked as a team of 7 and completed as much as we could in the 8 week timeframe. We explored using **Agile design process** and practiced daily **scrum meetings**. 

#### The goal of our project is to create a platform where citizens of San Francisco can report hazards to the city for cleanup. 

---

### Tools and Architecture: 

  ##### Front End:
     - Jquery
     - JavaScript
     - Bootstrap
     - CSS
  
  ##### Back End: 
     - Node.js
     - Express
     - MySQL

  ##### Google API's: 
     - Geolocation
     - Google Map API
     - ReCaptcha v2
     
---

### Features: 

   - Guest users without accounts can search, use the map, and view details of hazards in SF.
   - Users that are logged in can also submit a hazard report, including a description, picture, and location pin. 
   - Admins are given a special access token that allows for the ability to see pending hazards, and assign, or deny them. 
   - Once a hazard has been asigned by an admin it is visible to everyone. Admins can chane the status to 'completed' once the task is done.
   
---

<img width="1280" alt="Screen Shot 2020-02-12 at 3 14 36 PM" src="https://user-images.githubusercontent.com/43154475/74388819-3f040680-4db1-11ea-9160-1aa052850d14.png">

---

<img width="1280" alt="Screen Shot 2020-02-12 at 3 14 12 PM" src="https://user-images.githubusercontent.com/43154475/74388772-209e0b00-4db1-11ea-8f19-6bdea0522071.png">

---

<img width="1280" alt="Screen Shot 2020-02-12 at 4 29 44 PM" src="https://user-images.githubusercontent.com/43154475/74390115-21d13700-4db5-11ea-8ce7-b8916aac7ff2.png">

---

### Authentication:

  We used JSON webtokens along with cookies for validation. This gives a session to the user, checks for access control, and protects our database routes from malicious actors. 

- ### [Sample Design Document](https://github.com/T-mclennan/Summer-Project-2019/files/4195818/CSC648-848.Summer.2019.Milestone2.Team2.pdf?raw=true)
