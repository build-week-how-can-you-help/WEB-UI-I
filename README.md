# WEB-UI-I

Proposal

- What problem does your app solve? 
	*It matches people living or visiting an area with charities/non-profit organizations that match their interests/and abilities, making it easier to find volunteer opportunities. (Andrew Goenner)
	* (Nico) - matches people with charities they are most likely interested in.  As simple as typing what you are interested in and a direct line to charities in the area will be yours.

	It allows people to search a list of registered non-profits near them and give them information so they can determine if they want to help that non-profit or not. Info that can be given could be:
financial breakdown (tax info)
analysis of the institution itself
links to its website to find more information
User reviews


- Be as specific as possible; how does your app solve the problem?
Our app will solve this problem by hooking into a government database that lists all non-profits that are in a certain area code. If that is not possible, using some other open database. Last possibility is to have an admin and editors/moderators that can manually input that info or making it so orgs can register and place their data in themselves (in which case it there would need to be some sort of verification on our end to let that org officially be added or not)

(Nico) Our app will solve the problem by matching you to not only nearest available charities, but ones that most likely match your interests.  Simple and clean.

- What is the mission statement?
(Nico) Let’s make it easy to Give

Features

- What features are required for your minimum viable product?
	*A list of interest keywords that match with organization keywords (Andrew Goenner)
	
Pulling list of non-profits by zip or city.
login/logout
Search by keyword in zip/city
Display non-profit info:
Name
Website
Other info from database (once we find the database and what info it provides)
Registered user reviews (?)
	*(Nico) - Description/ paragraph of interests
 - Zip code/ area indicator
	
- What features may you wish to put in a future release?
	*Expand to reach all 50 states
Rating system
A analytical brakedown of non-profit financials (how much money goes to serving their cause, how much goes to administration both detailed and high overview like 7 cents/dollar goes to helping the homeless and 93 cents/dollar goes to paying administration, etc.)
Moderated review list of both positive and negative reviews. Ability to sort by positive or negative reviews.
Bullet list of top three positives and negatives of org (no org is perfect)


- What do the top 3 similar apps do for their users?
Category filtering
Profile creation/registration
What non-profits i’m interested in
What I can do
What days & times I’m  available
Give non-profit my details (phone, email, etc)
Sending matches to users
Have a list of non-profits uses can sort themselves with keep or delete
Ability to schedule days to show availabitily to non-profits
Notify friends of non-profits via email/social media (Sean)
Let non-profits
Add intro
Add org info
Contact info
Details of the event (indoor/outdoor, how you can volutneer etc)
Tags for people opportunity may appeal to (homeless, seniors, verterans, animals, etc)
List of skill for volunteer opportunities looking for
Requirements (must be 18 years or older, etc.)
email their app/website users about events coming up
Map of location of event
Listing of similar opportunities

Frameworks - Libraries

- What 3rd party frameworks/libraries are you considering using?
	*templates:
https://colorlib.com/wp/template/seelife/
	https://freewebsitetemplates.com/forums/threads/charity-template.2957/
	sematic-ui
- Do APIs require you to contact its maintainer to gain access?
- Are you required to pay to use the API? 
- Have you considered using Apple Frameworks? (MapKit, Healthkit, ARKit?)
For Data Scientists


- Describe the Established data source with at least rough data able to be provided on day 1. 
- You can gather information about the data set you’ll be working with from the project description. Be sure to collaborate with your PM, and your Backend Architect to chat about the resources you have.
(Nico) I have information on 318 charities in Maryland from data.gov. 
Name, description, address, phone and website is the information I chose to extract
- Write a description for what the DS problem is (what uncertainty/prediction are we trying to do here? Sentiment analysis? Why is this a useful solution to a problem?)
The DS problem to solve will be to match the description and area to the most similar charities accordingly.  
Use some sort of NLP model to get charity that matches description
From results, order by nearest to furthest from given location
- A target (e.g. JSON format or such) for output that DS students can deliver to web/other students for them to ingest and use in the app
JSON
Target Audience

- Who is your target audience? Be specific.
	*Those visiting or living in an area and searching for volunteer opportunities
- What feedback have you gotten from potential users?
- Have you validated the problem and your solution with your target audience? How?

Research

- Research thoroughly before writing a single line of code. Solidify the features of your app conceptually before implementation. Spend the weekend researching so you can hit the ground running on Monday.
Prototype Key Feature(s)

- This is the “bread and butter” of the app, this is what makes your app yours. Calculate how long it takes to implement these features and triple the time estimated. That way you’ll have plenty of time to finish. It is preferred to drop features and spend more time working on your MVP features if needed.

MVP for front-end:
Register
Login
User (user)
admin/editor (edit, update, add, delete non-profits)
Logout
Show a list of non-profits with (if given by API):
Non-profit name
Brief summary
Search by zip/city
Routes
Landing page
User login
Search page with form/input
Main list of filterable non-profits
Stretch:
User:
Short bio
Skills listing
Upload a photo
Categories interested in
Sign up for events & shifts
Non-profit:
Summary of org
Contact info
Name
Email
address
List days of activities with available shifts


MVP for BackEnd (global info) :
Login Endpoint for administrators to make edits/updates
Register Endpoint for administrators
Non-Profit List Access Endpoint
Restricted Routes for administrators
Data Model Structure based on info from data science
Ability for general user to have a favorites page
