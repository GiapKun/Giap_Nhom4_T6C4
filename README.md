# Hey! Nice to see you. 👋

I love to talk about travel ⚡ technology ⚡, I have a huge attraction on 🔭 Spacex 🔭. Connect with me here

- 🏢 I'm currently working at **The Mona Host** and studying at Huflit University
- 🚀 I use daily: **Python**, **Git**, **Docker**, **MongoDB**,  **VS Code**
- 💻 I work using: **Python**, **FastAPI**, **MongoDB**, **GitLab**, **Docker**, **Amazon AWS**, **PostMan**, **GitHub**

# Health Care 
This is a pet project of mine with a few friends in the same subject at Huflit University

## Tech
**Backend:** 
- FastAPI is a modern, high-performance, batteries-included Python web framework that's perfect for building RESTful APIs. </br>

**FontEnd:**
- React lets you build user interfaces out of individual pieces called components.

<h2>Table Of Content</h2>
<ol>
  <li><a href="#description">Description</a></li>
  <li><a href="#lat">Languages and Technology Used</a></li>
  <li><a href="#Req">Requirements</li>
  <li><a href="#features">Features</a></li>
  <li><a href="#steps">Steps to run the project in your machine</a></li>
  <li ><a href="#ws">Working-Snippets</a></li>
  <li><a href="#cs"> Database-Snippets</a></li>
</ol>
<h2 id="description">Description</h2>
HealthCare is a console based application which is built using java.This application helps in management of  Patients, doctors, admin in a easy and comfortable way.using this Application patients can quickly Sign up, Login, view his/her profile, view doctors, book Appointment, view Report, choose doctor, view Appointments, give feedback, pay online and logout. Admin can add Doctors,view patients list, view Doctors list,remove doctors, see feedback given by patients,view reports,logout. Doctor can login, view profile, viewAppointments, Attend Patients and logout. 

## Problem statement:
1. Patient logs in, uploads medical/lab test bills and submits it for insurance. Notifications are sent to hospital and lab admin.
2. Hospital admin logs in, verifies and approves the bills. This approval is stored on the smart contract
3. Lab admin approves the lab test bills. This approval is also stored on the smart contract
4. Once both of them approve, notification are sent to insurance admin.
5. Insurance admin can check for approvals of hospital and lab after which he will calculate the claim amount and do the claim.


## High Level System Architecture: 
 <img src="https://github.com/heshanera/HealthPlus/blob/master/screenshots/componentInteractions.png" alt="componentInteractions" width="100%">

<h2 id="features">Features</h2>
 <ul>
  <li><a href="#login">login</a></li>
  <li><a href="#Admin">Admin’s DashBoard</a></li>
  <li><a href="#Patient">Patient’s DashBoard</a></li>
  <li><a href="#Doctor">Doctor’s DashBoard</a></li>
  <li><a href="#Report">Report-Table</a></li>
  <li><a href="#Appointment">Appointment-Table</a></li>
  <li><a href="#feedback">Feedback Form</a></li>
  <li><a href="#Booking">Booking Appointment</li>
  <li ><a href="#choose">Choosing Doctor</a></li>
  <li ><a href="#Payment">Payment Process</a></li>
  </ul>

<h1 id="steps">How to run this project ?</h2>

# Backend
### Cloning the Repository

First, clone the repository from GitLab and navigate into the project directory:

```bash
git clone https://github.com/GiapKun/Health-Care.git
cd Health-Care
```

### Setting Up the Environment

1. Create a folder named `.env`:

```bash
mkdir .env
```

2. Create a file named `dev.env` inside the `.env` folder and fill it with the following content. You can get the `SECRET_KEY` from [this link](https://8gwifi.org/jwsgen.jsp) by selecting `HS512` and clicking "Generate JWS Keys". Then, copy the `SharedSecret`:

```plaintext
environment=dev
app_database_name=app
log_database_name=app
database_url=mongodb://db?retryWrites=true

# Authentication
SECRET_KEY={ENTER_YOUR_SECRET_KEY}
ALGORITHM="HS512"
DEFAULT_ADMIN_EMAIL={ENTER_YOUR_DEFAULT_EMAIL}
DEFAULT_ADMIN_PASSWORD={ENTER_YOUR_DEFAULT_PASSWORD}
```

3. Create a file named `test.env` inside the `.env` folder, and add the following content:

```plaintext
ENVIRONMENT=test
database_url=mongodb://db-test?retryWrites=true
```

### Install pre-commit

1. Download [pre-commit](https://pre-commit.com/):

```bash
pip install pre-commit
```

2. Install pre-commit

```
pre-commit install
```

### Running on Linux

To start the project on a Linux machine:

1. Open your terminal.
2. Navigate to the project directory.
3. Run the following command to make the script executable and start the Docker containers:

```bash
chmod +x bin/linux/start.sh
bin/linux/start.sh
```

### Running on Windows

To start the project on a Windows machine:

1. Open Command Prompt or PowerShell.
2. Navigate to the project directory.
3. Run the following command to start the Docker containers:

```cmd
bin\windows\start.bat
```

This script will build and start the Docker containers for the FastAPI application and MongoDB database.

### Accessing the API

Once the containers are up and running, you can access the FastAPI application by navigating to:

```
http://localhost:8001
```

You can explore the automatically generated API documentation at:

- Swagger UI: [http://localhost:8001/docs](http://localhost:8005/docs)
- ReDoc: [http://localhost:8001/redoc](http://localhost:8005/redoc)

### Stopping the Project

To stop the Docker containers, use the following commands based on your operating system:

#### Linux & Windows

Press `Ctrl + C`

This will stop and remove the containers, networks, and volumes created by Docker Compose.


# Fontend

## Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
