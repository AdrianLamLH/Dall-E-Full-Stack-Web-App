# Dall-E Image Generator Platform

## Description

This image-gen platform provides a web app built on a MERN stack that dynamically creates, hosts, and displays AI-generated images using OpenAIs text-to-image model Dall-E-2.
Backend hosted on Render, and frontend hosted on Vercel.

## How to use

Open [link](https://tinyurl.com/yw9am72f) to Vercel hosted Web App (given active deployment status):
1. Users can search through gallery of previous posts
2. Users can generate their own posts on the create page

    i. Subsequently, users can share their creations to the gallery

    ii. Each submission is labelled, and indexed by name & post prompt
4. Users can download any images from the gallery 


## Running the Application locally
#### Ensure [Vite](https://vitejs.dev/) is installed

Clone the Repository:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*(Use this commit: 0d5a4b1963e3149fcc210a0eca70fe80148fedad)*
##### `git clone https://github.com/AdrianLamLH/Dall-E-Full-Stack-Web-App.git DALL_E_APP`

##### `cd DALL_E_APP`

##### `npm install`

### To run the Frontend (ReactJS):

##### `cd client`

##### `npm run dev`

The app should be accessible at
[http://localhost:8080/api/v1/dalle](http://localhost:8080/api/v1/dalle) so you can view it in the browser.

### To setup the Backend:

##### Open a second command line to run the backend server.

##### `cd server`

##### Create a .env file in the server folder. Add your [mongodb](https://cloud.mongodb.com/), [openai](https://openai.com/blog/openai-api), and [cloudinary](https://cloudinary.com/) keys to the .env file like the following:
`MONGO_DB_URL=<YOUR_MONGO_DB_URL_HERE>`
`OPENAI_API_KEY=<YOUR_OPENAI_API_KEY_HERE>`
`CLOUDINARY_CLOUD_NAME=<YOUR_CLOUDINARY_CLOUD_NAME_HERE>`
`CLOUDINARY_API_KEY=<YOUR_CLOUDINARY_API_KEY_HERE>`
`CLOUDINARY_API_SECRET=<YOUR_CLOUDINARY_API_SECRET_HERE>`

##### Replace <YOUR_MONGO_DB_URI_HERE> with the MONGO_DB_URI you obtained from the database you created at https://cloud.mongodb.com/, similarly for the other services

### Afterwards, to run the backend (NodeJS and MongoDB):

##### `npm start`

This will run the backend on [http://localhost:8080](http://localhost:8080)

Once both the front end and backend are running, the application will be fully useable.
