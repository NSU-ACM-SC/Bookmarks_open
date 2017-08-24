# Bookmarks
### An image bookmarking web application
#### Developed as class project of CSE482: Internet and Web Technology Course in Summer 2017

## Introduction
Today’s web pages are filled with images. A lot of them. And while browsing the world wide web we often stumble upon images that we would like to save and show to others but the ways are a bit tedious. We need to download them, save them somewhere, then share. There are famous and effective photo sharing sites like flickr, instagram, imgur etc. but they lack this feature of saving an image from a web page without leaving the web page. We wanted to approach this problem in a different manner. We created an web application that on the back sits as a platform to store and show user images for later usage and also adds a follower system so that an user can follow what other people are sharing as well. We named this process bookmarking. Hence came the name of the app - Bookmarks.

## Features

- Easily login from Google, Twitter and Facebook

- A client side bookmark module for allowing the user to get images from webpages

- A social network system where users can follow each others and their bookmarked images


## Downsides
Currently the application can fetch images from websites using HTTP only. No support for HTTPS yet! (Part of future work)

## Bookmark process
The web applications has an web browser extension which can be saved as a bookmark in any web browser. So when user visits a web page and wants to bookmark images, he/she will click on the bookmark and without leaving the page a small window will appear containing all the images in the website that can  be saved and bookmarked. Clicking on the desired image will save it to the user’s profile in the application.

![Imgur](http://i.imgur.com/2XnWI4G.png)



## Following users and liking images
A user can visit another user’s profile and click on follow to start following.  Same for liking. Open the image and clicking on liking will do.

![Imgur](http://i.imgur.com/f4iXAxA.png)

## Dependencies

- `python3`
- `django`
- `pillow`
- `python-social-auth`
- `redis`
- `social-auth-app-django`
- `sorl-thumbnail`

Please check requirements.txt for version info of these packages.

## Making it work

- You need to have Redis up and running for this application to work. You can learn more at (https://redis.io)

- Prepare the python env using the requirements file. You can create virtualenv if you want to.

```bash
pip install -r requirements.txt
```

- Get inside the directory and run migrations before you start the app. After you're done doing migrations, start the server using `manage.py`.

- Once you're inside and have created your user and reached the dashboard, click on `BOOKMARK IT!` and drag it to your browsers bookmarks toolbar.
