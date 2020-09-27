
# Project Name : Nasa Picture Of The Day
> This project's main goal was to try React, and Nasa API 


### Screenshot
<br>
<img width="300" src="https://user-images.githubusercontent.com/56839789/94368295-9b6b2a80-00e3-11eb-96cb-25d82af6bae5.gif" alt="screenshot">

### Creating the React App
`npx create-react-app nasa-apod`
<br />
The npx command will install and run the command create-react-app
The last part of that command is the name of our app.
<br>
Then: `cd nasa-apod` And: `npm start`, Finally: head on over to `localhost:3000`

### Components:
- /Home.js
- /NasaPhoto.js
- /NavBar.js

### React Router Magic!
`npm install --save react-router-dom`
<br>
In here we see that we have imported the react-router-dom, our /Home and /NasaPhoto components, and set up the routing for that.

For the react-router-dom dependency, we pulled out BrowserRouter and Route for our routing.

BrowserRouter will wrap around our declared routes.
Route will help us build out our routes, what component the route will show, and how the URL route will look.

### NasaPhoto.js
We are using React Hooks so we see that for state, we have set it to null and later we set setPhotoData to the data we pull out of the API.

In the return() we are using photoData to use each element of the API in an organized way. We are using:

- Photo URL - That is the photo itself.
- Photo Title - That will be used as our alt for the photo and the h1 on our page.
- Photo Date - This will be the current date because this API is the Astronomy Picture of the Day.
- Photo Explanation - This will be a paragraph of information that NASA provides about the photo.

### Handling the media type
The API sometimes sends back a short video. So we want to be able to display that properly. If the media type is "image", we will return it as an image. If not, we will return the "image/video" in an <iframe />.


## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

### What I learn, pratice:
- create a React App
- react-router-dom
- set navbar in react
- router
- components
- fetch nasa api
- use .env variable (example fo APIkey)



