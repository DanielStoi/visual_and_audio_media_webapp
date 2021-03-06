# Visual and audio media webapp

## Credits
This was part of an group assignment at the University of Sydney,for the subject ISYS2120.

-Designed for the University of Sydney, School of Computer Sciences

-(Initial) Assignment Codebase by Harshana Randeni

-Initial Schema by Ryan Skelton

My group members and contributers where:

-David, Ben, Vigesh

### Demo
Here are a bunch of screenshots that show different functionalities of the webapp.

This is the home screen after logging in.

![home](https://github.com/DanielStoi/visual_and_audio_media_webapp/blob/main/demo%20images/cature%20home.PNG)

In addition to this, clicking on any of the menu icons on the top will take you to a list of all the media of the corresponding category (eg movies, tv shows, songs). Clicking on any of the media items in the main section will take you to a separate page that has all the details about that individual media item.

This is the search functionlity (can choose to search for movies, songs, tv shows, podcasts in a dropdown menu next to search).

![search](https://github.com/DanielStoi/visual_and_audio_media_webapp/blob/main/demo%20images/capture%20search.PNG)

Now that a bunch of media items are on the screen, you can click on any item to get all the relevent information about that individual item.

![song](https://github.com/DanielStoi/visual_and_audio_media_webapp/blob/main/demo%20images/cature%20song.PNG)

As seen from the above screenshot, the genres are listed for every media item. However, genres are also clickable, which takes you to a page that lists all the media items of that genre.

![genre](https://github.com/DanielStoi/visual_and_audio_media_webapp/blob/main/demo%20images/cature%20genre.PNG)

## Outline

The media server is designed to keep track of files and metadata information regarding
various audio and video media.

### Schema Description

![ERD](demo%20images/ISYS2120_a3_erd.png)
As per the above schema you have various consumable media:

1. Movies
1. TV Shows (which have TV Episodes)
1. Songs (which are performed by Artists and appear in Albums)
1. Podcasts (which have Podcast Episodes)

There is also some User Account information which contains information about the user
including:

1. Contact Methods
1. Username / password
1. Subscribed podcasts
1. Consumed media

We have abstracted most of the common elements such descriptions, artwork and genres
into a MetaData table system. The primary Metadata table contains 3 fields:

1. an ID field (which other tables use a FK)
1. a MetaData type ID field (which maps to the MetaDataType table)
1. an actual value for the metadata

Presently, there are 4 possible types of metadata:

1. Song Genre
1. Film Genre
1. Artwork
1. Description

# What we had to do within the assignment
In addition to the skeleton/structure of the program, some of the  functions, routes, and html templates where already completed. Essentially all of the server side (sql) code was done already, including the sample data. What the group added in reference to the server side code was password hashing and the ability to add songs and users, though SQL functions.

In the assignment, we had to code 10 tasks within the database.py file, which was a significant chunk of the database application programming code and acouple of routes in the routes.py file. This is in addition to modifing and creating templates that would be referenced by the routes.py functions to render the corresponding pages.

The group also added new functionalities, which involved adding functions to the database.py, routes.py files and creating html templates.


