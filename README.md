# Image Captioning WebApp with Clarifai

## Prerequisites

•	Basic knowledge of HTML, CSS, and JavaScript.
•	Sign up for a free Clarifai account to obtain an API key.
•	Sign up for a free GitHub account to create the repository.

## Set Up Your Project

•	Login to your GitHub account.
•	Create a new repository in GitHub to organise your project files.
•	Inside the repository, create an HTML file (‘index.html’) using the add file button.
•	Create a CSS file (‘styles.css’) for styling your webpage.
•	Create a JavaScript file (‘script.js’) for handling API requests and interactions.

## Build the HTML Structure

Create an HTML structure with a header, main content area, an input field for image url, a button to trigger captioning, an image container to display the uploaded image, and a paragraph to display the caption.

In your ‘index.html’ file, create the basic structure of your webpage:

#### code available in 'index.html'

## Style Your WebApp

In your ‘style.css’ file, add CSS rules to style the elements and make your webpage visually appealing.

## Add JavaScript Functionality

In your ‘script.js’ file, you’ll write JavaScript code handle image url, displaying image from url, and sending requests to Clarifai’s API. Here’s a simplified example:

### JavaScript Functions:
•	getBlipCaption(imageUrl): This function sends a request to the Clarifai Blip model to generate captions for an image URL.
o	It takes the ‘imageUrl’ as an argument.
o	Constructs a JSON request object with user and app ID, and the image URL.
o	Makes a ‘fetch’ request to the Clarifai API, using your PAT authentication.
o	Handles the response and calls ‘displayBlipCaption’ to display the generated caption.


•	displayBlipCaption(response): This function processes and display the caption received from Clarifai.
o	It checks if the response contains valid outputs.
o	Extracts the raw caption text from the response.
o	Displays the caption caption on your web app.


•	User Interaction: 
o	Add an event listener to the button with the ID ‘captionButton’. When clicked, this button triggers the ‘getBlipCaption’ function.
o	Inside the ‘getBlipCaption’ function, it fetches the image URL entered by the user in the ‘imageUrlInput’ field.
o	The image URL is then used as an argument to call ‘getBlipCaption’, which initiates the caption generation process.

## Sign up for a Clarifai Account

Visit the Clarifai website https://www.clarifai.com/ and sign up for a free account if you don’t already have one. You will need to provide email address and create a password.

### Create an Application

•	After signing in, click on your profile icon and select “My Apps” from the dropdown menu.
•	Click the “+ Create” button.
•	Give your application a name and description. Select primary input type to “Image/Video”. You can leave the other settings as default for this tutorial.
•	Click “Create App”.

### Obtain Your API Key

After creating the application, you will receive and API key. The key is essential for making API requests to Clarifai.

### Create Your Personal Access Token (PAT)

After obtaining your API key, head over to the security settings by clicking on the user image on top right corner of your dashboard. In this section, create a new PAT using the “Create Personal Access Token” link (refer below snippet).

### Deploy the WebApp

•	Configure GitHub Pages:
o	Go to your repository’s main page on GitHub.
o	Click on the “Settings” tab.
o	Scroll down to the “GitHub Pages” section in the left sidebar.
o	In the “Source” dropdown menu, select the branch containing your web app’s source code. Usually, you’ll choose the ‘main’ branch.
o	Click the “Save” button. GitHub Pages will now use the selected branch to deploy your web app.

•	Verify the Deployment:
o	After saving settings, scroll down to the “GitHub Pages” section again. You will see a message indicating the URL where your web app is deployed. It should look like: ‘https://yourusername.github.io/repositoryname’.
o	Click on the provided URL to access your deployed web app. You should see your web app running on GitHub Pages.



