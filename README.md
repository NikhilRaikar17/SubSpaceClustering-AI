# BreweryDB 

A simple two screen web app. One screen lists all the beers and another displays detailed information of a specific user clicked beer.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites

* [Create-react-app](https://github.com/facebook/create-react-app) 
* [NodeJs](https://nodejs.org/en/)
* [Bootstrap](https://getbootstrap.com/)
* [FontAwesome](https://fontawesome.com/how-to-use/on-the-web/using-with/react)
* [ExpressJs](https://expressjs.com/)

```
Give examples
```

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo
``` bash
.
+-- _config.yml
+-- _drafts
|   +-- begin-with-the-crazy-ideas.textile
|   +-- on-simplicity-in-technology.markdown
+-- _includes
|   +-- footer.html
|   +-- header.html
+-- _layouts
|   +-- default.html
|   +-- post.html
+-- _posts
|   +-- 2007-10-29-why-every-programmer-should-play-nethack.textile
|   +-- 2009-04-26-barcamp-boston-4-roundup.textile
+-- _data
|   +-- members.yml
+-- _site
+-- index.html
```

## Deployment

Add additional notes about how to deploy this on a live system

## Author

* **Nikhil Raikar** - *Initial work* - [NikhilRaikar](https://github.com/PurpleBooth)

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).




Brewery-app
  |-- public       # Python dependencies.
  |-- src/                   # Custom binaries.
      |-- components
      		|-- Details
      		|-- Listing
      		|-- main              # Cleanup the project.
      |-- img
      	|--
      	|--            # Change to debugging environment.
      |-- app.js             # Change to production environment.
      |-- app.css
      |-- index.js
      |-- index.css               # Setup the project.


# VacationTracker Web Application

## Introduction

This is a Web application for managing the vacation dates of employees as a 
self-service. The backend uses the Flask micro framework for Python based on 
Werkzeug and Jinja 2. The frontend uses the Bootstrap 4 CSS and JavaScript
framework and is based on the SB Admin Bootstrap admin template. For the 
database SQLite3 is used.

  * Flask: http://flask.pocoo.org/
  * Bootstrap: https://getbootstrap.com/
  * SB Admin: https://startbootstrap.com/template-overviews/sb-admin

## Requirements

This Web application requires the following software:

  * python3: Python interpreter version 3
  * python3-pip: Python module installer PIP
  * python3-venv: Python virtual environment
  * sqlite3: SQLite version 3 for the database export

Install this software as usual. Here is an example of installing it on Ubuntu.

  sudo apt-get install python3 python3-pip python3-venv sqlite3

## Project Structure

The project follows and extends the folder structure as expected by Flask.

  VacationTracker
  |-- LicenseManagement.py     # Main application file.
  |-- LicenseManagement.wsgi   # WSGI wrapper for Apache.
  |-- apache2-vhost.conf     # Apache virtual host configuration.
  |-- requirements.txt       # Python dependencies.
  |-- dev/                   # Custom binaries.
      |-- cleanup              # Cleanup the project.
      |-- debug_env            # Change to debugging environment.
      |-- prod_env             # Change to production environment.
      |-- setup                # Setup the project.
  |-- templates/             # HTML page templates supporting Jinja2.
      |-- base.html            # Base template for all pages except login.html.
      |-- licensedetails.html  # complete overview of licenses page.
      |-- login.html           # Login page.
      |-- overview.html        # License display page extending base.html.
  |-- static/                # Static page content.
      |-- css/                 # Custom CSS files.
      |-- js/                  # Custom JavaScript files.
      |-- images/              # Images and icons.
      |-- vendor/              # CSS and JavaScript frameworks.
  |-- venv/                  # Virtual Python environment.


## Development and Debugging

The application can be developed using just a text editor, or using the PyCharm
IDE or any other Python IDE supporting Flask. 

Setup the project by executing bin/setup from the project directory.

  cd LicenseManagement
  chmod a+x bin/*
  dev/setup

This is required only once to create the virtual environment, install Flask and 
its dependencies into the virtual environment, and to initialize the database. 

ATTENTION: If the database already exists, it will be deleted!

Flask comes with a built-in Web server that can be run in production (default) 
or development mode supporting application debugging. The application can be
run from the command line in debugging mode as follows.

  cd LicenseManagement
  . dev/debug_env
  run

If to run in production mode, execute following commands instead.

  cd LicenseManagement
  . dev/prod_env
  run
