<br/><br/><br/><br/>
# **Table of Contents**

1. Project Overview
2. Project Members and Roles
3. Diagrams
4. Scrum
5. User Guide
6. Tech Manual
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
# **Project Overview**

## Objective
* The overall objective of the project is to provide potential bus riders with a web accessible portal to view buses routes and their current locations, as well as payment for prepaid bus rides utilizing a ridership card one would swipe upon boarding a bus.

# System Functions
* The overall scope is to add a working user account system, integrating captcha, confirmation emails with sendgrid, text messages with twillio, and secure payment methods for bus rides through stripe.

## Ridership
* Utilizes a separate concrete library to allow for users to:
		* Purchase/be assigned individual rider cards
		* Allow for easy payment at a terminal mounted to the bus
		* Allow for greater amounts of data for future projects
* Dynamic ability to change touch point system by use of Dependency Injection best practices
	
## Payment

* Payment Integration
	*	Currently Stripe, but includes a payment library that can be used to integrate any form of payment available, such as Square, PayPal, and cryptocurrency


## Twilio 
*  Twilio uses Amazon Web Services to host telephony infrastructure and provide connectivity between HTTP and the public switched telephone network through its APIs, allowing the program to send text messages to the user.

## Sendgrid
* Sendgrid uses its API's to send users emails on demand, our use case has it sending messages to verify the users email account 

## Captcha
* Captcha is a type of challenge–response test used to determine whether or not the user is human, preventing spam accounts and hindering intrusion.

## Unit Testing
* Unit Testing is a level of software testing where individual units/components of a software are tested. The purpose is to validate that each unit of the software performs as designed.


___
<br/><br/>
<br/><br/>
# Project Members
| Member | Role |
| ------ | ------ |
| Gabrielle Ashley | Scrum Master |
| Aaron Williamson | Developer |
| Tanner Cude | Developer |
| Trevor Vieth | Developer |
| John Cunningham | Technical Lead |
| Mara Kinoff | Process Lead |


# Terminology 


## SCRUM

Scrum is the methodology used to develop this project. Scrum consists of five main events:

Sprint: these are the measurements of time or the deadlines. Each sprint for this project was two weeks long.

Sprint Planning: During this time the team collaborates to discuss the different tasks at hand as well as estimated story point values for each story.

Daily Scrum: In a work setting, these would be fifteen minutes meetings at the beginning of every day to discuss what each person worked on, what they will be working on, and if they had any roadblocks or errors that they need assisting with.

Sprint Review: The sprint review happens after each sprint to see how much the team has completed as well as any problems they had and how they fixed or plan to fix them, and what they will do next.

Sprint Retrospective: This is when the team has an opportunity to talk openly about the sprint. During this time they discuss what went well, what could be improved, and what they will improve later as well as give an overall feel of how they think the sprint went.

## SOLID

Single Responsibility Principle

Open Closed Principle

Liskov Substitution Principle

Interface Segregation Principle

Dependency Inversion Principle


## Description of Primary and Secondary Actors

  

Users:

- An over encompassing term that holds all users regardless of role in the system.

Riders:

- A term that describes the users that actively ride the buses.

Student:

- A type of rider that has a specific amount charged.

Adult:

- A type of rider determined by age that is charged a specific amount

Senior:

- A type of rider determined by age that is charged a specific amount

Paras:

- A type of rider that can request stops at their home out of city limits

Non-Riders:

- A term used to describe users that do not actively ride the buses

Admins:

- Non-Riders that have access to records and data from the website/application

Drivers:

- Non-Riders that drive buses and can be assigned stops for paras

Vehicles:

- A large term detailing both buses and para-transit vehicles

Buses:

- The vehicles that travel certain routes through the city

Para-buses:

- Vehicles assigned to specific stops requested by paras

Devices:

- Those actors that provide data

GPS:

- The tracking system attached to each bus that details the current location

POS:

- The Point Of Sales system that handles transactions from cards

Cards:

- The cards that are assigned to specific riders as a payment option

Routes:

- A list of stops that is traveled by a bus

Stop:

- A specific stop that a vehicle makes. May or may not be included in a route.

Database:

- The actor that holds the user’s data for the various actions they can take

----
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
<br/><br/><br/><br/>


# Diagrams

### Class
<img src="https://lh3.googleusercontent.com/FFa9tFD_lpuQFGomfUE3XWTg7ZmcDHzbY5yMZmuLSsfTOWEplVybBO5afNQlEgZwKp4LLH8nrpp3cA" alt="drawing" width="800"/>

 <br/><br/>

### ERD
<img src="https://lh3.googleusercontent.com/x6ye7-3VnTmnweMaLYKXLPE_Lcj4bJZrN5HxgizyGx5lBO2D7IBVWgzD3MLdoWNGpV1tbiC9VggIsQ" alt="drawing" width="800"/>

<br/><br/>
<br/><br/>

### Use Case

<img src="https://lh3.googleusercontent.com/4HJ3YkvWR4KVMt5xm_WURZROT9pD1qwzcFjir_ONuqJGatioX0rOJU3OJkXiPFTQ2DZPIWLWzrSRXA" alt="drawing" width="800"/>

<br/><br/>
<br/><br/>
<br/><br/>
<br/><br/>
<br/><br/>

### Activity

<img src="https://lh3.googleusercontent.com/axGNLl0Ml6zA2sET9453WHDDuqtrbNv0wYcQ4g2WRGQiz39RdWNAeF6KYQqGarXWIRDeo1jskg5vxg" alt="drawing" width="800"/>

<br/><br/>


### Sequence

<img src="https://lh3.googleusercontent.com/cp6WjhyEtcb_Ow6iWuDPrytoXr0IbGNBg2ie-3GjSK0bSt4uWdiFTNekkwVqS1idKbI1BHqr0-XDYA" alt="drawing" width="800"/>

<br/><br/><br/><br/>
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

### State

<img src="https://lh3.googleusercontent.com/iTOo6f8LIp1GcITWuzHul1vtCXQV2UzYBhtRfsMpWALbVpgGU29y7uTTx2LQycYiWoMEwYCmvWa1iw" alt="drawing" width="800"/>


<br/><br/>

----------
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

GENERAL STRUCTURE

  

-   Users
-   Riders
-   Adult
-   Students
-   Seniors
-   Paras
-   Non-Riders
-   Admins 
-   Drivers
-   Vehicles
-   Buses
-   Para-buses
-   Devices
-   GPS
-   POS
-   Cards
-   Routes
-   Stops
-   Database
----------

DEFINITIONS
- Routes are made up of stops
- Routes are independent of buses but require buses
----------

RELATIONSHIPS
-   Riders ride buses
-   Each type of rider pays a different amount
-   Paras can request stops
-   Buses are assigned to routes
-   Buses stop at stops
-   Drivers drive buses
-   Admins control the database
-   GPS tracks buses
-   Riders CAN use cards to pay
-   Cards are ASSIGNED to one rider
-   Cards allow riders to pay the POS
-   Para-buses aren’t assigned to routes
-   Para-buses travel to individual stops
----------
----------
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>


<img src="https://lh3.googleusercontent.com/ZRe4fCvuRKjriPV9LlUF4Pd8hCAfLTJ3gnGwYk0C-QlRytlnIi_Ui5lnhuuKOrD5oBVlWZrEYvmXCw" alt="drawing" width="800"/>


<img src="https://lh3.googleusercontent.com/MNKP1o383hogNj7G93ByNn6rD5Ij5RPrvEcO70W0dxJJaMKKQxVRYznfwnbtPJ2siQqbSaTPqiDctQ" alt="drawing" width="800"/>

<img src="https://lh3.googleusercontent.com/9CjUM6wHK7XwKhdz3FW4a_6CieBVKwYJhtliDyYIStukgv2xOc9izZ_omdKMJaO45OVenUZwEEbFLg" alt="drawing" width="800"/>

<br/><br/>
<br/><br/>
<br/><br/>

# Sprint 1
* Many of the backlogs and burndown charts became distorted as work items were migrated to new sprints as necessary.

<img src="https://lh3.googleusercontent.com/CMLL6gJEYd-9aCT7sCdH81w5IM6ZfXlC5guIZ_N_X3h402GI7ceAzBP2z2cO6Sp4ydQkpxpVz5pDFA" alt="drawing" width="800"/>

### Burndown

<img src="https://lh3.googleusercontent.com/tnPS26DKILiSnvhKaa41rUTByeE0t6BHXMhn4DWNw_AoXofwRi1-AJZ0vHPS5ONIa-B_Onpym1zcAA" alt="drawing" width="800"/>

## Sprint 1 Meeting 1 February 27 2019

  

### Gabby

What did you do yesterday?

-   I created the class diagram, and I started on the view for the home page
    

What are you doing today?

-   I am going to work on finishing the home page view
    

Is there anything holding you back?

-   Currently nothing
    

----------

  

### Tanner

What did you do yesterday?

-   Re-familiarized with ASP.NET/MVC
    
-   Skimmed through the code that we already have
    

What are you doing today?

-   Creating view for Login page
    
-   Creating ERD diagram
    

Is there anything holding you back?

-   Nothing
    

----------

  

### Aaron

What did you do yesterday?

-   I created the descriptions for primary and secondary actors, and added 5 features with the intention to associate those with the PBI’s due.
    

What are you doing today?

-   I will be working almost exclusively with Twilio and incorporating SMS messaging for our application.
    

Is there anything holding you back?

-   An extremely limited knowledge of Twilio, as I’ve only used it once before.
    

----------


  

### Trevor

What did you do yesterday?

-   Created use case diagram
    

What are you doing today?

-   Work on the register view
    

Is there anything holding you back?

-   Nothing right now
    

  

## Sprint 1 Meeting 2 March 1, 2019

  

### Gabby

What did you do last?

-   I added the css and js files to the devel branch which I will be pushing up tonight
    

What are you doing next?

-   Finish the home page tonight
    
-   Start email messages using sendgrid task
    

Is there anything holding you back?

-   Nothing so far
    

----------

  

### Tanner

What did you do last?

-   Created ERD
    
-   Created Login view
    

What are you doing next?

-   Begin the process of implementing the Captcha
    

Is there anything holding you back?

-   Nothing so far
    

----------

  

### Aaron

What did you do last?

-   SMS with Twilio. Nuget packages and etc.
    

What are you doing next?

-   More work with SMS and creating Navbar in _layout.html
    

Is there anything holding you back?

-   Twilio currently is configured for a different version of ASP.NET Core
    

----------

  

### Trevor

What did you do last?

-   Use cases, thought about the Registration view
    

What are you doing next?

-   The Registration view
    

Is there anything holding you back?

-   Nothing at the moment
    

  

## Sprint 1 Meeting 3 March 4, 2019

  
  

### Gabby

What did you do last?

-   I finished the home page
    
-   I started implementing sendgrid to work on email
    

What are you doing next?

-   Top 3 technical problems
    
-   Working on implementing sendgrid, re scaffolding for identity to get the correct files to show up to implement sendgrid
    

Is there anything holding you back?

-   Not being able to access the controllers and files needed to implement sendgrid
    

----------

### Tanner

What did you do last?

-   Worked with Google’s reCAPTCHA
    
-   Made Admin account and got our API keys
    

What are you doing next?

-   Top three technical problems
    
-   Fully implementing reCAPTCHA (or alternative, possibly)
    

Is there anything holding you back?

-   Need to continue reading on reCAPTCHA
    

----------

  

### Aaron

What did you do last?

-   I created the navbar in _layout successfully. There weren’t any issues with that as far as I have seen, and I have followed a few tutorials regarding Twilio with no luck currently.
    

What are you doing next?

-   I plan to follow more Twilio tutorials over the next couple of days as well.
    

Is there anything holding you back?

-   There are multiple Twilio tutorials and they tend to say different things. As of this point, I’m trying to hit on one that is correct for our version of ASP.NET and our project in general.
    

----------

  

### Trevor

What did you do last?

-   Worked on Registration
    

What are you doing next?

-   Finishing Registration
    

Is there anything holding you back?

-   Life

# Sprint 2

<img src="https://lh3.googleusercontent.com/fGwb6tN9n2yVFlb8LEg7ztivsnyLl3XyK7ROLbLY_5i3q0BDYmBwFa6jij5QrwTpFbgcPfyRCvIfng" alt="drawing" width="800"/>

### Burndown

<img src="https://lh3.googleusercontent.com/vEq3dY4f_68UkhGtPbZzoQLua7t8A3vx3i7BJp7wSvFb3Sxw5iPb3uThX_wNvkXeO68qGp2kNcWsuA" alt="drawing" width="800"/>

## Sprint Meeting 1 March 8th 2019

### Gabby

What did you do last?

-   4390 homework, planned sprint 2
    

What are you doing next?

-   Get sprint one changes into master branch, deploy to azure, fix sendgrid bug
    

Is there anything holding you back?

-   Sendgrid issue with identity causing a blockage
    

----------

  

### Tanner

What did you do last?

-   Planned Sprint 2
    
-   Familiarized myself with Twilio
    
-   Found helpful Youtube video
    

What are you doing next?

-   Attempting to implement what I found in Twilio video into my code
    

Is there anything holding you back?

-   No
    

----------

  

### Aaron

What did you do last?

-   Looked through John’s repository and documentation for Twilio
    
-   Planned Sprint 2
    

What are you doing next?

-   Attempting to get a test text message working
    

Is there anything holding you back?

-   Time constraints
    

----------

  

### Trevor

What did you do last?

-   Sprint two planning, believe I was able figure out how to integrate views in the new identity scaffolding.
    

What are you doing next?

-   Views
    

Is there anything holding you back?

-   No
    

  

## Sprint 2 Meeting 2 March 11 2019

  

### Gabby

What did you do last?

-   Read ch 3 of agile text book, research issues with sendgrid
    

What are you doing next?

-   Looking more into smtp and implementing the smtp class into project
    

Is there anything holding you back?

-   Lack of familiarity with sendgrid, errors
    

----------

  

### Tanner

What did you do last?

-   Became more familiar with the libraries and how we will structure those going forward
    

What are you doing next?

-   Attempt at more code implementation of Twilio and messing around with some of the libraries
    

Is there anything holding you back?

-   Continuing to experiment with Twilio
    

----------

  

### Aaron

What did you do last?

-   Read over Scrum guide PDF and looked through Twilio documentation from John
    

What are you doing next?

-   Going to work with Twilio and hopefully implement a quick and dirty version
    

Is there anything holding you back?

-   Not anything in particular, time constraints regarding family time.
    

----------

  

### Trevor

What did you do last?

-   Looked over sendgrid a bit, continued to be annoyed by identity.
    

What are you doing next?

-   Working on identity/view modification with gabby
    

Is there anything holding you back?

-   Nothing that has not already been mentioned. Time.
    

  

## Sprint 2 Meeting 3 March 13 2019

  

### Gabby

What did you do last?

-   Created sendgrid library and researched the issues
    
-   Created SLN at the project level
    

What are you doing next?

-   Create the sendgrid class
    

-   Add in API key for that
    

-   Create interface for sendgrid
    

Is there anything holding you back?

-   Lack of knowledge in not ever having to do this so far
    

----------

  

### Tanner

What did you do last?

-   Toyed around in Twilio and became more familiar with how we will need to set up our libraries
    

What are you doing next?

-   Work with Aaron in assisting him going forward
    

Is there anything holding you back?

-   Continuing to familiarize myself with Twilio and its API
    

----------

  

### Aaron

What did you do last?

-   Successfully sent a text SMS message
    

What are you doing next?

-   Attempt to create secret keys rather than having our API keys out in the open as it currently is.
    

Is there anything holding you back?

-   I’ve never worked with secret keys so that is new to me
    

----------

  

### Trevor

What did you do last?

-   Worked on getting power and computer to work
    

What are you doing next?

-   Continuing to pursue last meeting’s goal
    

Is there anything holding you back?

-   Time
    
-   Power outages
    

____________________________________________________________

## Sprint 2 Meeting 4 March 15 2019

  

### Gabby

What did you do last?

-   Read more about dependencies and interfaces
    

What are you doing next?

-   Create the sendgrid class
    

-   Add in API key for that
    

-   Create interface for sendgrid
    
-   Pushing sprint one to azure
    

Is there anything holding you back?

-   Lack of knowledge in not ever having to do this so far
    
-   No power since Wednesday, just got power back as of today
    

----------

  

### Tanner

What did you do last?

-   Toyed around in Twilio and became more familiar with how we will need to set up our libraries
    

What are you doing next?

-   Work with Aaron in assisting him going forward
    

Is there anything holding you back?

-   Continuing to familiarize myself with Twilio and its API
    

----------

  

### Aaron

What did you do last?

-   Looked over John's documentation about hiding the keys
    

What are you doing next?

-   Attempt to create secret keys and implement it as a library
    

Is there anything holding you back?

-   Time constraints
    

----------

  


### Trevor

What did you do last?

-   Got working power and computer.
    

What are you doing next?

-   Implementing Login/Registration
    

Is there anything holding you back?

-   Time
    
-   Power outages
    
## Sprint 2 Meeting 5 March 18 2019

  

### Gabby

What did you do last?

-   Hooked up sendgrid, got a test email sent out
    
-   Attempted to integrate into identity
    
-   Worked on the glossary
    

What are you doing next?

-   Getting sendgrid to hook up to identity
    

Is there anything holding you back?

-   Other classes
    
-   Debugging is not working right in vscode
    
-   Not getting right results
    

----------

  

### Tanner

What did you do last?

-   Preparing for midterm
    
-   Worked on glossary
    
-   Continued working with Twilio
    

What are you doing next?

-   Assist in getting things pushed to Azure
    
-   Get SMS working completely
    

Is there anything holding you back?

-   Other classes
    

----------

  

### Aaron

What did you do last?

-   Worked on Glossary, and looked at Twilio some
    

What are you doing next?

-   Attempt to create secret keys and implement it as a library
    

Is there anything holding you back?

-   Interviews and midterms this week
    

----------

  

### Trevor

What did you do last?

-   Succeeded in implementing Login/Registration
    

What are you doing next?

-   Fix slight format errors
    
-   Assist Team endeavors
    

Is there anything holding you back?

-   Time

# Sprint 3

<img src="https://lh3.googleusercontent.com/sEhzL2d0XsvvlypixupR3ogYhvmf7psvIdvP7Vn3mKXOud-9sgISUllOmlN1Zv_atnNLZnW1BNKn-Q" alt="drawing" width="800"/>

### Burndown

<img src="https://lh3.googleusercontent.com/byWG41rj0t_bsZn59aAc4Fws9DHFkubG7g6BSgUpdvd3wKAe-O9G3qUXkrxYF9nu-AXJnIp_pwgcYA" alt="drawing" width="800"/>

## Sprint 3 Meeting 1 March 25th 2019

### Gabby

What did you do last?

-   I got my register.cshtml.cs file working again so that a user can register
    
-   Merging changes from sprint one into master branch
    
-   Sprint 3 planning
    

What are you doing next?

-   Continue merging sprint one changes into master
    
-   Get sendgrid working
    

Is there anything holding you back?

-   Currently do not have anything holding me back
    

----------

  

### Tanner

What did you do last?

-   Looked over the code for the nav bar in the shared folder
    

What are you doing next?

-   Attempt to cannibalize some code from the PRPC website to make the nav bar. Whatever is missing, I will add in
    

Is there anything holding you back?

-   No
    

----------

  

### Aaron

What did you do last?

-   Nothing at all.
    

What are you doing next?

-   Implementing secrets.json and incorporating library for Twilio.
    

Is there anything holding you back?

-   Internet went out on Thursday and I won't have a tech out until Tuesday. I do have a light week homework wise so I can make up the slack.
    

----------

  

### Trevor

What did you do last?

-   Competed previous sprint. Found YouTube series that appears to have the info I need for identity roles and how to utilize/implement them.
    

What are you doing next?

-   Watching the vids and implementing roles.
    

Is there anything holding you back?

-   Inexperience.
    

  

## Sprint 3 Meeting 2 March 27 2019

### Gabby

What did you do last?

-   I merged GabbySp1 into devel, TannerSprint1 into devel
    
-   I updated devel branch
    

What are you doing next?

-   Merge Trevor’s sprint one branch into devel
    
-   Merge devel into master
    
-   Continue to work on sendgrid
    

Is there anything holding you back?

-   Currently nothing
    

----------

  

### Tanner

What did you do last?

-   Began working on getting nav-bar working
    

What are you doing next?

-   Continuing to work on nav bar and successfully getting it working
    

Is there anything holding you back?

-   Not at the moment
    

----------


  

### Aaron

What did you do last?

-   Nothing as internet still hasn’t begun working yet. After another call with Suddenlink, they will send a maintenance team out tomorrow from 2 - 4
    

What are you doing next?

-   The same as last time. I will create additional libraries for Twilio and include the secrets.json file
    

Is there anything holding you back?

-   The internet still won’t work until tomorrow afternoon
    

----------

  

### Trevor

What did you do last?

-   Watched most of the vid series way too late at night only to discover it was similar but not quite the right thing. It did give a bit of related knowledge though.
    

What are you doing next?

-   Ultimately I found what should be a more applicable guide to follow. So, that.
    

Is there anything holding you back?

-   Finding the correct info, knowledge base.
    

  
  

## Sprint 3 Meeting 3 March 29 2019

  

### Gabby

What did you do last?

-   Spent a lot of time working with SendGrid, I have gotten it to work now, there is validation that is occuring with the email
    

What are you doing next?

-   Merging Trevors sprint 1 branch into devel
    
-   Working with the database connection strings and then getting what we currently have published to azure
    

Is there anything holding you back?

-   Nothing yet
    

----------

  

### Tanner

What did you do last?

-   Tried to figure out how to get some of the PRPC website’s javascript working for the dropdown on the nav bar
    

What are you doing next?

-   Get the nav bar working. Will consult other resources
    

Is there anything holding you back?

-   Figuring out the site’s code
    

  ----------


### Aaron

What did you do last?

-   Created the library for SmsService
    

What are you doing next?

-   Trying to implement it correctly with interface and fix the problems
    

Is there anything holding you back?

-   There’s an error about the using statement for SmsService
    

----------

  

### Trevor

What did you do last?

-   Researched Identity rolls, there is a lack of documentation for it. Most all of it has to do with mvc on its own without identity as we’re using it at least
    

What are you doing next?

-   Apparently being told that it was all for naught
    

Is there anything holding you back?

-   Pointless work.
    

____________________________________________________________

## Sprint 3 Meeting 4 April 2 2019

### Gabby

What did you do last?

-   I researched dbcontext
    
-   Started working on concrete class implementation and database calls
    

What are you doing next?

-   Continue making the database calls and start testing their implementation
    
-   Make a unit test to test the database calls
    

Is there anything holding you back?

-   Currently nothing
    
----

  

### Tanner

What did you do last?

-   Mostly recovered from being sick
    

What are you doing next?

-   Finish what I had left
    

Is there anything holding you back?

-   Making sure I’m getting rest
    

----------


  

### Aaron

What did you do last?

-   Solved the problems with the library and the dependency injection.
    

What are you doing next?

-   Implementing with Identity/begin with unit testing depending on what we hear tomorrow in class.
    

Is there anything holding you back?

-   Knowledge about unit testing, but we’re covering it soon anyway
    

----------


  

### Trevor

What did you do last?

-   Learned that identity is being abandoned, moved on to working on the ridership card input setup, mostly done.
    

What are you doing next?

-   Finalizing the input setup, unit testing
    

Is there anything holding you back?

-   Unit testing
----

## Sprint 4 Meeting 1 April 5 2019

<img src="https://lh3.googleusercontent.com/braXf7gbFUV0LjaGCA4KLp7T9Rwry_3V57Eui4TbdSnuQHH50wzWr66ku6nxHe2DLM-IIDIA8-Q2tw" alt="drawing" width="800"/>

### Burndown

<img src="https://lh3.googleusercontent.com/5bjR7QG8Ru0xx4AYeyTDldyKsdaF0Kwqj7MkjugWJMC3Sox3Q_EskpTq7wcJbwshWOVeIBgqEtvK-A" alt="drawing" width="800"/>

### Gabby

What did you do last?

-   In the process of fixing devel branch and then merging into master branch
    

What are you doing next?

-   Fixing devel branch and then merging changes back in
    
-   Work on getting ridership card updated and working
    

Is there anything holding you back?

-   Checking and testing devel to make sure the branch is working properly
    
-   Having an http 400 authentication tokenry error when submitting a form on the website, have to fix this issue before merging to master branch--this prevents pushing to azure until the issue is fixed
    

----------

  

### Tanner

What did you do last?

-   Implemented reCaptcha for the Login and Register pages
    
-   Worked with Trevor to ensure that the drop down now works (Thanks Trevor)
    

What are you doing next?

-   Assist in getting pushed to Azure
    

Is there anything holding you back?

-   Will possibly have to wait for merging stuff to take place before I can do so
    

----------

### Aaron

What did you do last?

-   Looked into SmsSender class similar to EmailSender that was generated
    

What are you doing next?

-   Look into Stripe API implementation and make an initial attempt
    

Is there anything holding you back?

-   No previous knowledge of Stripe
    

----------

  

### Trevor

What did you do last?

-   Finished Card Reader, Map Setup, Fixed Navbar Styling and Dropdown
    

What are you doing next?

-   Azure, updating ridership card view to handle the payment process
    

Is there anything holding you back?

-   Knowledge base
    



  

## Sprint 4 Meeting 2 April 8 2019



### Gabby

What did you do last?

-   Today I am fixing devel, I’ve got my own personal branch running
    
-   Had no internet this weekend so I wasn’t able to work on anything
    

What are you doing next?

-   Create a new devel branch that is correct
    

Is there anything holding you back?

-   Currently nothing
    

----------

  

### Tanner

What did you do last?

-   Set up a resource pool and published a web app within azure. App is running.
    

What are you doing next?

-   Get code pushed up to Azure on our web app
    

Is there anything holding you back?

-   Need to re-familiarize myself with some of Azure
    

----------
----------

  

### Aaron

What did you do last?

-   Worked with Stripe and got it to work with test cards but not in a separate library
    

What are you doing next?

-   Attempt to incorporate Stripe into a library
    

Is there anything holding you back?

-   I think it’ll be similar to Twilio and Sendgrid, but I’m not sure
    

  ----------


### Trevor

What did you do last?

-   Successfully switched over to and connected to new database, worked on views.
    

What are you doing next?

-   Continuing the work on the card interface, misc views/formatting.
    

Is there anything holding you back?

-   Not at the moment.
    


  

## Sprint 4 Meeting 3 April 10 2019

### Gabby

What did you do last?

-   Solved issues relating to the http 400 error (turns out that it was breaking on a user not being confirmed through email which is why that specific user could not sign in)
    
-   Merged changes in the master, master now has sendgrid, recaptcha, and the views for the home page, login, and register
    

What are you doing next?

-   Hoping back on the ridership card
    

Is there anything holding you back?

-   Nothing so far
    

----------

  

### Tanner

What did you do last?

-   Made a bit more progress in Azure
    
-   Began the process of getting into unit testing
    

What are you doing next?

-   Push code to Azure
    
-   Begin unit testing
    

Is there anything holding you back?

-   Continue to gain knowledge in unit testing
    


----------

  

### Aaron

What did you do last?

-   Created a class library for payment, then had to remove it due to Babb’s requirements
    

What are you doing next?

-   Implement a payment class and interface that works along the same architecture as his
    

Is there anything holding you back?

-   I need to study and understand his example ridership example more
    


----------

  

### Trevor

What did you do last?

-   Worked on acct mgmt formating, attempted to figure out how to make the navbar more compatible with the various pages
    

What are you doing next?

-   Continuing the same. Looking into twilio
    

Is there anything holding you back?

-   Twilio
    


  

## Sprint 4 Meeting 4 April 12 2019

### Gabby

What did you do last?

-   Playing with twilio, need account information to register phone number for testing
    

What are you doing next?

-   Ridership class and logic, looking at dr babb code and trying to incorporate it
    

Is there anything holding you back?

-   Nothing so far
    

----------

  

### Tanner

What did you do last?

-   Prepared to deploy code to Azure
    
-   Began developing a unit test
    

What are you doing next?

-   Finish unit test
    
-   Get code pushed to Azure
    

Is there anything holding you back?

-   Not at the moment
    

----------

  

Aaron

What did you do last?

-   Research regarding Dr. Babb’s code and finding ways to incorporate Stripe in as a concrete class
    

What are you doing next?

-   Attempt to create a concrete Stripe class and interface
    

Is there anything holding you back?

-   Understanding of Babb’s code and time
    

----------

  

### Trevor

What did you do last?

-   Looked at twilio a bit
    

What are you doing next?

-   navbar/formatting/twilio research
    

Is there anything holding you back?

-   Time
    

----------
# Sprint 5 Meetings


<img src="https://lh3.googleusercontent.com/B22y1V7YC3zMu20BJ8wYRFwN7ZROrWeZRjAGeMX0SK8TsVphNHaEBfwoFE9dP8Z7iXOeWvgjjYcjZg" alt="drawing" width="800"/>

### Burndown

<img src="" alt="drawing" width="800"/>

# ** //------NEED TO ADD AT COMPLETION OF SPRINT------ ** 

## Sprint 5 Meeting 1 April 19 2019

### Gabby
What did you do last?

-   Sprint planning, setup work
    
-   Made a devel3 branch
    
-   Merged all of the branches for sprint 4
    

What are you doing next?

-   Continue to work on ridership card concrete class and interface
    
-   Delete old branches (obsolete)
    

Is there anything holding you back?

-   Nothing so far
    

----------

  

### Tanner

What did you do last?

-   Pushed everything to Azure
    
-   Got API linked with Azure
    

What are you doing next?

-   Unit testing
    

Is there anything holding you back?

-   Refamiliarize myself with unit testing a bit but nothing really at this point
    

----------

  

### Aaron

What did you do last?

-   Worked on the sprint planning with Gabby
    

What are you doing next?

-   Changed the stripe MVC over to Razor pages
    

Is there anything holding you back?

-   Time
    

----------

  

### Trevor

What did you do last?

-   Sprint review, planning
    

What are you doing next?

-   Helping with dashboard View Model, dashboard views/controllers
    

Is there anything holding you back?

-   View model will need to be done before views/controllers are able to be completed
    

  

----------

  
  

## Sprint 5 Meeting 2 April 22 2019

### Gabby

What did you do last?

-   Worked on concrete class implementation of ridership, finished the ridership interface, and working on the controller and views for ridership
    

What are you doing next?

-   Finish the controller and views and perfect the concrete class implementation for creating a ride
    

Is there anything holding you back?

-   Currently nothing
    

----------

  

### Tanner

What did you do last?

-   Began writing some for the unit testing
    

What are you doing next?

-   Completing unit testing
    

Is there anything holding you back?

-   Not at the moment
    

----------

  

### Aaron

What did you do last?

-   Changed the view for Payment and the general structure with a PaymentController
    

What are you doing next?

-   I discussed with Gabby about the next steps. Start with user roles.
    

Is there anything holding you back?

-   Understanding of Identity
    

----------

  

### Trevor

What did you do last?

-   Meeting for Project documentation framework
    

What are you doing next?

-   Project documentation
    

Is there anything holding you back?

-   Those parts that will require information I do not have.
    

----------

  

## Sprint 5 Meeting 3 April 24 2019

### Gabby

What did you do last?

-   Implemented a ridership history table, and bus card sign up feature and a bus card riding simulation
    

What are you doing next?

-   Implementing two tables, last minute touch up of ridership features
    
-   Integrate ridership and stripe
    

Is there anything holding you back?

-   Nothing so far
    

----------

  

### Tanner

What did you do last?

-   Continued to work with unit testing. Went over Mara’s github
    

What are you doing next?

-   Continuing to work on unit testing
    

Is there anything holding you back?

-   Not at the moment
    

----------

  

### Aaron

What did you do last?

-   Worked with Payment by manipulating the views to only show Payment pages when a user is logged in.
    

What are you doing next?

-   Using Gabby’s code as a template to create a database that holds the correct information and work with her to create a ViewModel.
    

Is there anything holding you back?

-   A general lack of experience with databases, but with Gabby’s code base, I feel confident.
    

----------

  

### Trevor

What did you do last?

-   Project Documentation
    

What are you doing next?

-   Project Documentation
    

Is there anything holding you back?

-   No
    

----------

  
  

## Sprint 5 Meeting 4 April 26 2019

### Gabby

What did you do last?

-   Finished ridership individually, worked with Aaron on the start of integrating ridership and stripe
    

What are you doing next?

-   Working on the method that subtracts money when a person wants to ride the bus
    

Is there anything holding you back?

-   Nothing so far
    

----------

  

### Tanner

What did you do last?

-   Continued unit testing
    

What are you doing next?

-   Continuing unit testing
    

Is there anything holding you back?

-   No
    

----------

  

### Aaron

What did you do last?

-   Worked alongside Gabby in creating the viewmodel and formulating a plan of attack for the next steps.
    

What are you doing next?

-   Gabby and I are meeting Sunday to finish up the code, and I'd like to have the presentation finished and the reload card finished.
    

Is there anything holding you back?

-   Understanding of the code created today.
    

----------

  

### Trevor

What did you do last?

-   Familiarized myself with the notebook overview
    
-   Need to put it in markdown
    

What are you doing next?

-   Talking with team members about relevant information regarding parts of the project that will be going into the binder
    

Is there anything holding you back?

-   Nothing at the moment.
    

----------


# User Guide
* To view bus routes and locations a user must simply access the map tab from the navbar.

* To create an account a user must select the register tab from the navbar, enter their information, satisfy the captcha, click register, and complete email confirmation.

* To login a user must select the login tab from the navbar, enter their credentials, satisfy the captcha, and click login. 

* To modify account details a user must select account, modify the desired details within its section, and save.

* To sign up for a bus card, initiate a ride, view ride history, load your card, or check card balance, simply access the related tab from the navbar.

---

# Tech Manual
* Clone the repo from Github
* Obtain Stripe, Captcha, Twilio, and Sendgrid API keys
* For local projects, insert API keys within appsettings.json or the related .cs file for non secret implementation
	* else create a separated secrets.json file for the project to utilize 
* Create a MySql database
* Connect to database with your server connection strings within appsettings.json and startup.cs
* Run dotnet restore
* Follow the Azure documentation for publishing the project ([https://docs.microsoft.com/en-us/azure/app-service/deploy-local-git](https://docs.microsoft.com/en-us/azure/app-service/deploy-local-git)
* Insert API keys into Azure
----


---
