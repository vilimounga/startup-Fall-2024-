# Fitness Tracker
## Specification Deliverable
### Elevator pitch
Have you been looking for a good reason to exercise and accomplish your health goals? The new Fitness Tracker makes it easy for users to record their daily steps and calories. As users record their numbers daily, users will see a simple graphic of their progress as well as a daily motivational quote! This simple tracker makes it fun and easy for users to see their progress while achieving their health goals.
### Design
![Image of the Fitness Tracker Web Application](images/trackerdesign.jpg)
### Key Features
- Secure User Login
- Display of 2 fitness metrics.
- Ability to enter personal health data
- Inputs entered are recorded over time
- Display of their data on a simple easy-to-read graph(s).
### Technologies

I am going to use the required technologies in the following ways.

- **HTML** - Uses HTML for website application structure. 3 HTML pages, one for login, one for inputting data, and one for viewing progress over time.
- **CSS** - Application adjusts for good viewing on various screens. CSS used to display colorful designs and shapes and eye-catching symbols.
- **React** - Provides login, choice display, and use of React for routing, components and redeveloping this application in this framework.
- **Service** - Backend service with endpoints for:
  - user login
  - retrieving fitness data
  - submitting daily fitness data
- **DB/Login** - Store users fitness data (steps and calories) in database. Register and login users. Credentials securely stored in database. Can't enter fitness data without authentication.
- **WebSocket** - As a user enters their daily fitness data, they'll receive notifcations of other user's steps for the day.
## HTML deliverable

For this deliverable I built out the structure of my application using HTML.

- [x] **HTML pages** - Three HTML page that includes the main/login page, recording fitness data page, and viewing progress page.
- [x] **Links** - The login page automatically links to the recording page. The recording page links to the progress page.
- [x] **Text** - Each of fitness data type is represented by text. Graphs uses textual descriptions.
- [x] **Images** - I include a free icon for web application. I added an image to the record HTML page.
- [x] **DB/Login** - Input boxes and submit/create button for login. The graphs represent personal data pulled from database.
- [x] **WebSocket** - While users is inputting data, notifications will pop up showing other user's data from that day.
- [x] **3rdPartyServices** - Quote on progress page is a placeholder for a 3rd party request for daily motivational quotes.