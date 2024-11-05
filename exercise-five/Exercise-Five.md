# Exercise Five: Creating an API

The purpose of this exercise is to get used to GETting and POSTing data to an API.

## Requirements:

1. Have a deployed Node app
2. Have a Firebase database
3. Have a place to view data
4. Have a place to write data through a form

## Directions:

1. Create new Github Repository (named "Dynamic Web Exercise Five")
2. Create and set up a new Node server (see Exercise 4)
3. Connect Firebase to the Node app (web code)
4. Create a Cloud Firestore database in Firebase - put on test mode for easy integration but you can use production if you are comfortable changing security settings.
5. Create a schema in Firebase for blog posts (include title, text, and author)
6. Setup a query from Firebase for an individual article (based on ID)
7. Setup a query from Firebase for all articles
8. Setup a route for each article
9. Setup a route for all articles
10. Create an html form in a route that has an action which posts to your API
11. Deploy to ??? (more information incoming)
12. Submit the link to the Github repo AND the link to the deployed server to James at ja155@nyu.edu or through Brightspace

## Useful Resources

_Note:_ Focus on "web" instead of Node for this project. Node will take you deeper into the Google Cloud Platform (which is more secure and scalable but outside of the scope for this exercise)

[Firebase Setup in JavaScript](https://firebase.google.com/docs/web/setup?authuser=0)

[Firebase Config Object](https://firebase.google.com/docs/web/setup?authuser=0#config-object)

_Note_: You will get your config object directly from Firebase admin panel in project settings. Just copy that and paste it in,

[Firestore Get Started](https://firebase.google.com/docs/firestore/quickstart)

[Firebase Read & Write Data](https://firebase.google.com/docs/firestore/query-data/get-data)

[Firebase Set Data](https://firebase.google.com/docs/firestore/manage-data/add-data)

[MDN - Node Forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/forms)

[Deploy to Render](https://www.freecodecamp.org/news/how-to-deploy-nodejs-application-with-render/)

### Extra Resources

[Firestore Quickstart GitHub Repo](https://github.com/firebase/quickstart-js/tree/master/firestore) : This might contain some useful code but note that it is not the same as the exercise. Keeping this here for future knowledge
