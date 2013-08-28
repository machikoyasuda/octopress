---
layout: post
title: "day two - enter Firebase"
date: 2013-08-27 21:41
comments: true
categories: development
---

Today:
- Did not go back into Cloudbees.
- Moved repository to GitHub instead, and started using a Node.js webserver for development.
- Hooked up Firebase to the Angular project and started adding items to Firebase database with my first controller.
- Wrote a few short JavaScript functions to (1) see how many items there are, (2) see how many are remaining and (3) calculate and show the progress.
- My model is as follows, at the moment: An array of item objects, which have a name (text) and status (true/false). False is not done. True means it's checked and done. 

Road blocks:
- GUID URL generation and persisting into database. I will need to (1) create a new URL for each new checklist, (2) save that ID into the database with the array of items with statuses and names. When a user returns to that specific URL, the user will see that same list. It will not refresh and go blank (like it currently does).
- Have not done any test-writing yet. But I want to! I've been writing in Sublime Text, console.log() into console and running the app. I would like to test, though.
- Down the line, we need to figure out how to deploy - Heroku or GitHub pages?

Tomorrow:
- I hope to set up testing somehow, with Jasmine, Karma or whatever.
- I hope to start saving and persisting data, even if I don't have unique URLs yet.

Code challenges:
- To make up for what I didn't do yesterday, I did a Ruby exercism.io and a JavaScript one.
- I will push them to GitHub as soon as they are approved.
