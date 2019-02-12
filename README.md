# Calls for Social Good 
<img src="https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/000/760/000/datas/gallery.jpg" width="400" alt="calls for social good homepage">
<img src="https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/000/760/017/datas/gallery.jpg" width="400" alt="add a reminder page">
<img src="https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/000/760/018/datas/gallery.jpg" width="400" alt="picture of text from calls for social good">

# Inspiration
In this day and age, reminders have become automated to the point of losing their effectiveness as a tool for accountability. Especially in the area of health, remembering to take medications or needing to check in with the elderly has lost its personable touch. Calls for Social Good solves this problem by anonymously putting you on the phone with a live person to ensure your well-being.

# What it does
Routines provide much needed support for the repetitive tasks in our lives. Whether it's waking up in the morning to go to work or school, taking our pills and essential vitamins for heart health, or remembering to go on a walk after a long day of sitting down, it's nice to have reminders to hold ourselves accountable. Eventually, we all get bored and tired of doing our repetitive tasks. They get muddled down in whatever work we engulf ourselves in and get lost along with our other New Year's resolutions or life goals. We realized that though we have reminders and alerts, it is not enough to hold us accountable. As human-beings, we are deeply moved with the social interactions of our daily lives. Our solution to this problem is Calls for Social Good. CSG aims to apply a more personal approach with reminders. Instead of getting a notification reminding you to take your medications, you receive a phone call from someone who has taken time out of their day to talk to you. We feel that this added relationship will hold people accountable for the things they need to do in their lives. When someone chooses your reminder to call, Calls for Social Good will text the person an anonymous phone number to call when it comes time to remind you. We do this all while still maintaining the privacy of both parties’ phone numbers. They can check in with you to make sure you’ve taken your meds and are doing alright. We even have an emergency contact feature where, an emergency contact of your choosing can be texted if the call does not go through and there is no call back within a certain time frame.

# How we built it
The entire infrastructure is designed around a custom REST API. The API is built on a Flask backend and deployed to Google Cloud. Our reminder and user data is all stored in the NoSQL Google Firestore. The calling features Twilio API Calls and multithreading to allow scheduling the SMS to the volunteer at a certain time. The frontend is built on React and deployed separately to interface with the custom API endpoints.

# Challenges we ran into
A major challenge was maintaining session objects across subsequent API calls using cookies on the frontend. Additionally, scheduling the threading for texting a volunteer at a specific time while avoiding race conditions proved to be more difficult than anticipated. Additionally, deploying to Google App Engine was a new experience for us. Despite the steeper learning curve, however we found this to be much more valuable.

# Accomplishments that we're proud of
We are proud to have deployed, which is typically not a step we take in our hackathons. Additionally, we tested all of our API endpoints and implemented error handling cases to minimize friction. Finally, the overall design and UI of our front-end is A E S T H E T I C. :)

# What we learned
Designing the front-end from its bare foundation provided a solid opportunity to polish up on React. Also, deploying with Google App Engine using NoSQL Firestore was a learning experience throughout.

# What's next for Calls for Social Good
Setting up infrastructure for screening and approving new volunteers. Additionally providing the option to view call history if either party wants to prefer to be matched for future calls.

# Built With
react, flask, twilio api, python, javascript, google-app-engine, google-cloud, firestore

# Teammates
https://github.com/fernanlukban <br/> https://github.com/karmitdandona <br/> https://github.com/VietDinh17
