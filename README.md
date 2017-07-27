# analyticsSimulator
Simple realtime analytics simulator


 


Scenario:



Consider a website that generates 2 types of events:

  - user logged in

  - user logged out



Task:



Design a system that in realtime can extract statistics about the users of the site.

Create a small CLI dashboard, that on each 10 seconds will display:

- average number of users

- number of unique users

- average time a user spends on the site (optional)


Notes:



  - a user can login and log out at any time

  - the order of the events is always logged in, logged out

  - the user logged in event has 3 fields: timestamp, user_id, session_id

  - the user logged out event has 3 fields: timestamp, user_id, session_id

  - the session_id identifies a specific user session on the site and is unique


 


Implementation details:


  - the system should be written as a simulation

  - only JDK 8 classes are allowed to be used in the implementation

  - the format of the output (dashboard) should be simple text




Deliverable:


  - a Java 8 command line application that simulates the website events and prints on the console the specified statistics

