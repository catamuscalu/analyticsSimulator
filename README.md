# analyticsSimulator
Simple realtime analytics simulator


 


Scenario:


Given a website that produces 2 types of events (user login and user logout), this one needs a realtime analytics system that can emit several statistics about the website traffic.



Task:

How would you design such a system, given that you need to output the following metrics about the website traffic in 10 seconds windows:

- number of unique users connected (unique user_id)

- average user session duration

At the end of the exercise, display the number of unique users since the beginnning of the simulation.

Consider offering a CLI dashboard that can emit these metrics each 10 seconds.



Notes:


  - a user can login and log out at any time

  - the order of the events is always logged in, logged out

  - the generated events have 4 fields and the following format: timestamp, event_type, user_id, session_id

  - the session_id identifies a specific user session on the site and is unique. A given user_id can generate one or more session_ids.
  
  - think of a simple implementation that should not take more than a couple of hours to complete, in the "production-ready" philosophy




Implementation details:


  - the system should be written as a simulation

  - the format of the output (dashboard) should be simple text
  
  - account for an optimal speed of ingestion from multiple sources of data
  - use the given simulation-input.csv input to test your simulation, considering that the test data has the following format: offset in seconds since start of simulation, event type, user_id, session_id
  


Deliverable:


  - a Java command line application that consumes the website events and prints on the console the specified statistics

  - Java compliance level required :  JDK 8
