# Async Week


#### MC1

Q: Which of the following libraries can be used to implement authentication in node applications?

* express-session
* cookie-maker
* passport
* passport-google-oauth

#### MC2

Q: Which of the following accurately describes the difference between hashing and encryption?

* Hashing is only used in data structures, whereas encryption is used in security.
* Hashing text is slow, but harder to reverse engineer (making it ideal for storing passwords), and encryption is fast, but easier to reverse engineer
* Hashed text is always a 40 character hexadecimal string, but encrypted text could be of any length
* Hashing text is a one-way operation (i.e. the original text cannot be reverse-engineered), but encrypted text can be reverse engineered (with the appropriate key).

#### MC3

Q: Which of the following describe ways to protect your application secrets (such as an API key)? Select ALL THAT APPLY

* Use all-uppercase letters for the variables that contain app secrets (i.e. GOOGLE_API_KEY)
* Use environment variables to store the values of app secrets
* Exclude any secrets from your git-tracking (by leveraging a .gitignore)
* Require your secrets from another module

#### MC4

Q: How do you prevent improper access in a web application (i.e. prevent non-admin users from taking actions that should only be available to admins)?

* On the front end: hide admin controls and pages unless the logged-in user is an admin
* On the server: send error responses for requests that only admin should be able to make, unless the user on the session is an admin
* Both A and B are important, but A is more important because otherwise the user experience is really awkward
* Both A and B are important, but B is more important because anyone can bypass your front-end and make requests to your API with curl

#### MC5

Q: What is a cookie?

* A persistent connection between a server and an individual client
* An object that lives in memory on the server that contains a dictionary with information about visitors to that server
* A small piece of data associated with a certain hostname that gets stored by a browser and sent with subsequent HTTP requests to that hostname
* Delicious!