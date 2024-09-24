# MyAwesomeApp

A simple tool to help organize your tasks and boost productivity. The app is designed to streamline daily workflows by letting users track tasks, set reminders, and prioritize to-dos in one place.

## Table of Contents
- [Description](#description)
- [Getting Started](#getting-started)
  - [Dependencies](#dependencies)
  - [Installing](#installing)
  - [Usage](#usage)
- [Deployment](#deployment)
- [Roadmap](#roadmap)
- [Version History](#version-history)

## Description

**MyAwesomeApp** is a web-based task management application built to help users stay organized. The app allows users to create tasks, assign priority levels, and set deadlines. Whether you’re managing personal to-dos or team projects, this app ensures that no task slips through the cracks. The app is built with modern web technologies, including React, Node.js, and MongoDB, and is optimized for both desktop and mobile use.

## Getting Started

### Dependencies

* Node.js v14.x or higher
* MongoDB (local or cloud instance)
* Any modern browser (Chrome, Firefox, etc.)
* Operating System: Windows 10 / macOS / Linux

### Installing

1. Clone the repository:
    ```bash
    git clone https://github.com/username/MyAwesomeApp.git
    ```
2. Navigate to the project directory:
    ```bash
    cd MyAwesomeApp
    ```
3. Install dependencies:
    ```bash
    npm install
    ```
4. Set up environment variables (create a `.env` file in the root directory):
    ```bash
    MONGODB_URI=your_mongo_db_uri
    PORT=5000
    ```

### Usage

* To start the development server:
    ```bash
    npm run dev
    ```
* Open your browser and go to `http://localhost:5000` to see the app in action.
* To run tests:
    ```bash
    npm run test
    ```
* To run the app in production:
    ```bash
    npm start
    ```

## Deployment

[Link to the project](#usage)

The app is deployed on **[Render](https://render.com)** for both the frontend and backend services, utilizing the platform’s free plan. The MongoDB database is hosted using **[MongoDB Atlas](https://www.mongodb.com/atlas)**, also on a free tier.

Here’s how the deployment is structured:
- **Frontend**: Deployed as a static site on Render, built from the `main` branch.
- **Backend**: Deployed as a Node.js API service on Render, using the `main` branch for automatic deployment.
- **Database**: Hosted on MongoDB Atlas, connected to the backend via the `MONGODB_URI` environment variable.

The deployment process on Render is automated, so anytime code is pushed to the `main` branch, the site and API are automatically updated. The steps for deployment were:
1. Set up two services on Render (one for the frontend and one for the backend).
2. Link each service to the GitHub repository.
3. Add environment variables (e.g., `MONGODB_URI`) in the Render dashboard.
4. Push code to the `main` branch for automatic deployment.

If you want to run the app on another platform (like Heroku or Vercel), similar steps can be followed—just ensure your environment variables are set properly for your database connection.


## Version History

* [v0.2]()
    * Added basic CRUD for posts
    * Added routes for register and login
* [v0.1]()
    * Initial Release
