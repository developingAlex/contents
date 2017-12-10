# Coder academy exercises
List of exercises worked through in class and what was covered in them. A quick reference for when I can't remember in what exercise a particular competency was covered (there was a lot)

(a lot of the rails exercises I haven't yet put on github, though git was used at the time, I will work on adding them whenever I have a spare moment)


# Javascript
* [CodePen exercise](https://codepen.io/webdevalex/pen/GOPNqB) - coding react-like functionality from scratch (watch the case-sensitivity on those javascript method names!)

# NodeJS & Express & MongoDB
## [nodeserver-first-lesson](https://github.com/developingAlex/nodeserver-first_lesson) - 20171122
* Uses an **api** to pull appropriate data for a given input (**postcodes**) 
* demonstration of **dynamically changing css** values (eg. about page header colour changes to whatever is entered in the url:
        localhost:7000/aboutred or localhost:7000/aboutblue etc       
* demonstration of different **mimetypes in json** responses
* JSON **stringify**
* introduces **REST client** VS Code extension and .http file for request testing
* serving up a wombat **gif**
* notes on running a server from a home pc which is accessible externally

## [express-mongoose-music-app](https://github.com/developingAlex/express-mongoose-music-app)- 20171124
* introduces model **validations**
* **CRUD**
* **Nodemon**
* **routes** and **routing**

## [react-flight-booking](https://github.com/developingAlex/react-flight-booking) - 20171127AM
* first **React**
* commands to initially install react on your computer
* Customising browser for react debugging 
* Sending parameters to components to determine what they give you back

## [react-bootstrap-components](https://github.com/developingAlex/react-bootstrap-components) - 20171127PM
* **React**
* practice making html components - components that implement the css library bootstrap
* intro to components so some information regarding them from pat in the code comments

## [emoji-dos2](https://github.com/developingAlex/emoji-dos2) - 20171128
* **React**
* a todo list that uses emojis and logic to indicate number of oustanding todos
* splits the todo list into two separate lists (in order to appear as though the list is being sorted) and just 'hides' corresponding entries from each list such that only the completed entries appear in one list, and only the incomplete entries appear in the next list, though both iterate over the same array of entries.
* programmed to be more **functional**, **immutative**.
* **Callbacks** and **function passing**
* introduces **components** for UI elements

## [linkedin-profile-editor](https://github.com/developingAlex/linkedin-profile-editor) - 20171129
* **React**
* demonstrates **form** usage to tie together two separate elements (image url input field and button).
    * If the field for the image url was programmed the same as the name fields it would have attempted to load an image for every alteration of a character in that field as the user typed, I wanted it to not do that as it would break the image as soon as the user started typing. I wanted instead for there to be a button they could click once they were finished typing in the url to their avatar image.
    * Original implementation had the button not tied to the input element in any way. The button invoked a method which then went and **retrieved the value of the element's current state.**
    * the subsequent implementation had the button and the input field tied together in a form. in that way when the button was pressed, the form was submitted, and the value of the input element was retrieved from the one bit of data that came through on the form submission. 
    * this approach is considered better than the original (though not as obvious in this situation) as it helps to encapsulate the information that is being worked with. As opposed to going and trying to read the current state of distinct elements, which could get messy if problem got more complex than this example.
* user declaration '**syntax sugar**' example
* introduces internal **state**

## [react-api-stockprice-app](https://github.com/developingAlex/react-api-stockprice-app) - 20171130
* **React**
* Using stock quote **api**
* **Axios** for http requests
* distinctions between 'get' and 'fetch'
* first time use of **componentDidMount**
* **event handlers**
* notes on pitfalls **passing data through to components**
* using && to **conditionally render elements**
* notes on arrays in state
* rendering with **.map**
* notes on return statement restrictions

## [storms-of-december](https://github.com/developingAlex/storms-of-december/tree/alex-master) - 20171205
* **React**
* **Node.js**
* app behaves like an api responding to URL requests with appropriate data.
* MongoDB seed
* distinct backend and frontend folders
* gitignore
* validators in models
* yarn scripts
* model attributes defaults
* seed file code techniques
* mongoDB mongoose operators to return a range
* mention of lodash
* process.exit

## [lakedisappointment](https://github.com/developingAlex/lakedisappointment) - 20171206
* **React**
* handling authentication in Node with **Passport** 
* handling authorization with **JWT**
* authentication **Middleware**
* linking up of **React** frontend with **Node.js** backend
* used **cors** to get around frontend server to backend server communication issues
* Used the **populate** method to get the object referenced by the attribute of another object
* covers database **object relationships**
* Discusses the MongoError: **E11000 duplicate key** error collection
* implements **CRUD** functionality
* **"how to run"** instructions in README
* MongoDB **seed** file
* package.json file has good example of **yarn scripts**
* Mongo terminal **db querying** and maintenance commands
