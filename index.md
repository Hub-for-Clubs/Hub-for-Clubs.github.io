## Table of contents

* [Overview](#overview)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)
* [Walkthrough videos](#walkthrough-videos)
* [Example enhancements](#example-enhancements)
* [Acknowledgements](#acknowledgements)

[Hub for Clubs](https://hub-for-clubs.meteorapp.com/)

## Overview 

Club Hub is a web application that provides a centralized directory for UH Manoa student clubs. UH Manoa students can login to browse a well organized directory of all current student clubs, with brief descriptions, meeting times and locations, URLs to their websites (if any), contact information for officers, and a few select photos. This project utilizes the following technologies:

* [Meteor](https://www.meteor.com/) for Javascript-based implementation of client and server code. 
* [React](https://reactjs.org/) for component-based UI implementation and routing.
* [Semantic UI React](https://react.semantic-ui.com/) CSS Framework for UI design.
* [Uniforms](https://uniforms.tools/) for React and Semantic UI-based form design and display.

## User Guide

This section provides a walkthrough of the Club Hub user interface and its capabilities. 

### Landing Page

The landing page is presented to users when they visit the top-level URL to the site. 

### Navbar

Contains links to the following pages:
* Home
* Club Explorer
* Sign up/Sign in

### Index pages (Projects, Profiles, Interests)

Club Hub provides three public pages that present the contents of the database organized in various ways. 

The Clubs page shows all the current defined Clubs and their associated Projects and Interests:

The Projects page shows all of the currently defined Projects and their associated Profiles and Interests:

Finally, the Interests page shows all the currently defined Interests, and their associated Profiles and Projects:

### Sign in and sign up

Click on the "Login" button in the upper right corner of the navbar, then select "Sign in" to go to the following page and login. You must have been previously registered with the system to use this option:
 
Alternatively, you can select "Sign up" to go to the following page and register as a new user:

### Home page
  
After logging in, you are taken to the home page, which presents a form where you can complete and/or update your personal profile:
* List of clubs the member is a part of
* Club announcements
* Personal information
* Interests
* Major
* A Bio
* Delete Account

### Club Explorer page

Given a list of all the clubs in the RIO database, by default in Alphabetical order. Options for filtering will exist, by type, subject, club specificity of major, and name. Clubs can either be joined by the user, or required to fill an application.

### Club page(s)

Is essentially the same as a home page, but with some changes:
* Has a join button
* Contact info for the Admin
* Announcements

### Club Admin page(s)

Has the ability to manipulate the following:
* Control club membership
* Change page info
* Change club tags
* Post announcements
* Share admin privileges
* View Club membership 
* R E M O V E C L U B button (in case of 86)

### Site Announcement Board

Admins can post freely to the site announcement board, but club owners may post only once per week, though they may edit and delete them. Posts from club owners will appear here and on their pages.

## Developer Guide

This section provides information of interest to Meteor developers wishing to use this code base as a basis for their own development tasks. 

### Installation

First, [install Meteor](https://www.meteor.com/install).

Second, visit the [Club Hub application github page](https://github.com/Ok-Boomer/Ok-Boomer.github.io), and click the "Use this template" button to create your own repository initialized with a copy of this application. Alternatively, you can download the sources as a zip file or make a fork of the repo.  However you do it, download a copy of the repo to your local computer.
  
Third, cd into the bowfolios/app directory and install libraries with:

```
$ meteor npm install
```

Fourth, run the system with:

```
$ meteor npm run start
```

If all goes well, the application will appear at [http://localhost:3000](http://localhost:3000). 

### Application Design

Bowfolios is based upon [meteor-application-template-react](https://ics-software-engineering.github.io/meteor-application-template-react/) and [meteor-example-form-react](https://ics-software-engineering.github.io/meteor-example-form-react/). Please use the videos and documentation at those sites to better acquaint yourself with the basic application design and form processing in Bowfolios.

### Data model

## Initialization

The [config](https://www.youtube.com/watch?v=dQw4w9WgXcQ) directory is intended to hold settings files. The repository contains one file: [config/settings.development.json](https://www.youtube.com/watch?v=dQw4w9WgXcQ).

This file contains default definitions for Profiles, Projects, and Interests and the relationships between them. Consult the walkthrough video for more details. 

## Quality Assurance

### ESLint

Hub for Clubs includes a [.eslintrc](https://github.com/bowfolios/bowfolios/blob/master/app/.eslintrc) file to define the coding style adhered to in this application. You can invoke ESLint from the command line as follows:

```
meteor npm run lint
```

ESLint should run without generating any errors.  

It's significantly easier to do development with ESLint integrated directly into your IDE (such as IntelliJ).

## Development History

The development process for Hub for Clubs conformed to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314f19/modules/project-management/) practices. In a nutshell:
 
* Development consists of a sequence of Milestones. 
* Each Milestone is specified as a set of tasks.  
* Each task is described using a GitHub Issue, and is assigned to a single developer to complete. 
* Tasks should typically consist of work that can be completed in 2-4 days.  
* The work for each task is accomplished with a git branch named "issue-XX", where XX is replaced by the issue number. 
* When a task is complete, its corresponding issue is closed and its corresponding git branch is merged into master. 
* The state (todo, in progress, complete) of each task for a milestone is managed using a GitHub Project Board.

The following sections document the development history of Hub for Clubs.

### Milestone 1: Mockup development

### Milestone 2: Data model development 

### Milestone 3: Final touches

## Walkthrough videos

## Acknowledgements

Thank you to [Phillip Johnson](https://github.com/philipmjohnson) for documentation formatting and [Branden Ogata](https://github.com/bsogata) for grading it.

