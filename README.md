# Udagram Image Filtering Microservice

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

## Cloning the Project
**1. Open your terminal**

**2. Navigate to the location you want the project to be**

**3. Clone the repository**
##### Note: Be sure to have Git installed on your workstation
>**Follow this link to install Git if you do not have it installed already. [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
>Proceed to cloning if you already have Git installed** 
```
git clone https://github.com/CalebAckom/udacity-image-filter.git
```

**4. Open the project in your IDE or Editor... Visual Studio Code is recommended**

**5. Run the commmand below to install all packages**
>**Note: Follow this link to get Node running on your machine. If you have Node JS installed already, skip this and install the packages** 
[Node](https://nodejs.org/en/download/)
```
npm install
```

**6. You are ready to start the application locally now. Run the command below**
```
npm run dev
```

**7. Create a new branch  from 'dev' branch and start contributing**
```
git checkout -b <branch-name>
```

**Happy Coding**

## Endpoint URL
```
http://image-filter-starter-code-dev2222222222222222222222.us-east-1.elasticbeanstalk.com/
```

The project is split into three parts:
1. [The Simple Frontend](https://github.com/udacity/cloud-developer/tree/master/course-02/exercises/udacity-c2-frontend)
A basic Ionic client web application which consumes the RestAPI Backend. [Covered in the course]
2. [The RestAPI Backend](https://github.com/udacity/cloud-developer/tree/master/course-02/exercises/udacity-c2-restapi), a Node-Express server which can be deployed to a cloud service. [Covered in the course]
3. [The Image Filtering Microservice](https://github.com/udacity/cloud-developer/tree/master/course-02/project/image-filter-starter-code), the final project for the course. It is a Node-Express application which runs a simple script to process images. [Your assignment]

## Tasks

### Setup Node Environment

You'll need to create a new node server. Open a new terminal within the project directory and run:

1. Initialize a new project: `npm i`
2. run the development server with `npm run dev`

### Create a new endpoint in the server.ts file

The starter code has a task for you to complete an endpoint in `./src/server.ts` which uses query parameter to download an image from a public URL, filter the image, and return the result.

We've included a few helper functions to handle some of these concepts and we're importing it for you at the top of the `./src/server.ts`  file.

```typescript
import {filterImageFromURL, deleteLocalFiles} from './util/util';
```

### Deploying your system

Follow the process described in the course to `eb init` a new application and `eb create` a new environment to deploy your image-filter service! Don't forget you can use `eb deploy` to push changes.

## Stand Out (Optional)

### Refactor the course RESTapi

If you're feeling up to it, refactor the course RESTapi to make a request to your newly provisioned image server.

### Authentication

Prevent requests without valid authentication headers.
> !!NOTE if you choose to submit this, make sure to add the token to the postman collection and export the postman collection file to your submission so we can review!

### Custom Domain Name

Add your own domain name and have it point to the running services (try adding a subdomain name to point to the processing server)
> !NOTE: Domain names are not included in AWS’ free tier and will incur a cost.
