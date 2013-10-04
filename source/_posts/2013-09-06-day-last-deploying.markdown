---
layout: post
title: "day six: deploying"
date: 2013-09-06 10:27
comments: true
categories: angular firebase github deploying
---
## How to deploy an AngularFire - Yeoman project to GitHub

1. Follow these instructions at [Yeoman](http://yeoman.io/deployment.html)
2. If you get fatal CRLF errors, install [dos2unix](http://linuxcommand.org/man_pages/dos2unix1.html). Type into Terminal: ```brew install dos2unix``` and then, use the tool to convert your troublesome files in the ```dist``` folder by running: ```find /dist -type f -exec dos2unix {} +```. This will convert all the files for you, without changing the filenames.
3. Make sure that your ```dist``` folder is in the root directory.
4. After your ```dist``` folder is added to the ```gh-pages``` branch, push it by running: ```git subtree push --prefix dist origin gh-pages```. This should push only your ```dist``` folder to your ```gh-pages``` branch. You should have an ```index.html``` in the root.
5. Go to ```your-name.github.io/your-repo-name```
6. Enjoy!

## A weekly stand-up:

#### What I did this week -
1. Thanks to **Theresa** for having us over at her house this weekend. Climbing takes my mind off all the stress.
2. I worked on three roadblocks in my project: a Firebase refreshing problem and not getting tests to run and deploying.
3. Yesterday I went to a mini-Madison Ruby meet-up in LA. It's always fun to meet other web developers in the area that really care about the community, ethics and the future of the Internet in general.

#### Roadblocks I faced this week -
1. Thanks to **Josh** helped me fix my refreshing bug. *Takeaway*: If you're creating new Firebase collection upon a button click, **separate the functions into different controllers**.
2. Thanks to **Delmer** for helping me move Firebase call from the controller to the service. This helped me get Jasmine/Karma tests to run. *Takeaway*: **Separate your Firebase into a service**.

#### What's next -
1. Now that I've deployed, I can start doing real testing on my phone and other people's non-iPhones. This will hopefully inform how I can continue to improve the user experience of typing, clicking, checking things off.
2. I also want to work on my datamap project and my personal portfolio page.
