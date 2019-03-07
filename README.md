The Monkees Jukebox website
By Giovanni Roberto Franzan

In this project, I tried to have some fun with creating original features that I thought could work well with the overall vibe of the website and its users. I did a little bit of research into the target audience which gave me some inspiration and guidance for the creation of these features. I hope the website gives somewhat of a nostalgic but also fun vibe to its users.

UX
User stories:
-> As an older fan of the Monkees, I’d like to re-listen to their greatest hits so that my mind may travel back to those days
-> As a soon-to-be wife/husband , I’d like to try and book the Monkees to play at my wedding ceremony

To me, designing a website for a band, that probably has a fanbase which is on average older than me, required me to do some “out of the box” thinking. The main question I had in my mind was, what would these users want?

**I’m writing this README file just a few short days after Peter Tork’s tragic passing, which resulted in a downpour of comments in the Monkees’ Youtube videos and social media.


Todd bob 5 days ago
This was back when life was good..... RIP PETER TORK.﻿

Noel K 5 days ago
We were all young once and the lucky few remain young forever in our hearts. R.I.P. Peter Tork and thank you for the happy music memories.﻿

Se7enwonders 5 days ago
Rest In Peace Peter.  Yet another part of my childhood gone.  But the music will live forever.

Journeyman 2 years ago (edited)
God please take me back to this time of my childhood magical days! 
:)﻿

Bruce M. 5 days ago (edited)
By By Peter you now join Davy, R.I.P. both of you. I watched the show every week when I was a youngster and still enjoy their music.﻿


What I got from my research, was that there was a real feeling of nostalgia when fans listened to the Monkees’ tracks. A nostalgia for a simpler time, when people all over the globe, would walk into a bar and put a coin in the jukebox and it would start playing the song they wanted.

The first piece of advice given by Steve Schoger & Adam Wathan in their Refactoring UI book is to start with a feature, not a layout.

A website or an app, is a collection of features, and before these specific parts (which we call features) are designed, a (web) developer lacks enough information to be able to design the layout of the whole website.

I will personally go further and argue that specific features can define a website and make it more memorable as a whole, much more than following a specific layout, which may or may not be ultimately appropriate for the project.


Features:

Jukebox feature

Nothing, to me, represents a jukebox (the feature I set out to design), like a vinyl record. So the first thing I did, was to go online (specifically Codepen) looking for examples.
The first good example I stumbled upon was the “Vinyl Color Test” by Antoine Lnit as this had almost exactly the final look I wanted for my vinyl records. (https://codepen.io/madmax_furycode/pen/GYQxXV?page=1&)
I polished it slightly by removing the vinyl-img item-2 image source and modifying the filter to get a light grey colour.

After I was happy with the overall look of the vinyl, I started researching how I could get the vinyl to play a specific track, chosen by the user, and that was when I hit my first roadblock; I didn’t understand Javascript. Luckily I found another Codepen which seemed to have the characteristics I wanted in my jukebox feature. This codepen example was “Vinyl Pure CSS” by Alexandre Broudin (https://codepen.io/AlexandreBroudin/pen/IfKFu) and it seemed to contain all of the Javascript I needed for my project. Little did I know at this point that it would have taken me a moderate amount of time to get these two Codepens to somehow merge into one and work together. One of the biggest issues I faced, as a new web-developer was that I had to merge specific bits of code from the two CSS files, especially since “Vinyl Pure CSS” was designed in SASS and I had to use the SassMeister website to convert this back onto normal CSS. After many mistakes and hours spent debugging code I finally had a working vinyl record with a PLAY button on it, which was able to play “I’m a believer” by The Monkees. Hooray!! (I guessed..)

At this point, I realised that having a single picture of a record with a play button on it, was nothing really similar to a ‘60s jukebox. I knew I wanted to design something that would be able to play a few different records from the Monkees, but I did not know what this would look like on the screen. It was then that my I went back to google and started looking for what a stack of vinyls could look like on a webpage but found nothing that was very interesting. I went back to CodePen, and searched for ”stack of cards” and “photo stack”, hoping that something useful would come out of it. And finally, this was when I found “Snap Stack” by the Appnotist (https://codepen.io/TheAppnotist/pen/oJMwZK). I initially thought this could work really well as a way of stacking records on the same page. After many more hours of trials later, however, I came to the realisation that the particular arrangement pattern on that Codepen was not going to work for my website, and it would have become a very confusing experience for the user. 

I did, however decide to keep the way in which the photos would rotate, once hovered over by the user (on desktop) and decided to design this feature with a simpler linear arrangement for the vinyl records. I then added all of the remaining vinyls, and connected each to a specific MP3 file, which I went on to store in the music/ folder.

Youtube videos and gifs

Following this, my second priority was to include some live footage of The Monkees playing in front of different crowds and in different settings. I thought it would be really important to show them playing live, as this may be one of the deciding factors for someone trying to hire the band to play at an event. I really liked the “Video within Modals” component I found on MDBootstrap (https://mdbootstrap.com/plugins/jquery/video/) as this allowed me to place 3 videos next to each other on larger screens and for them to “pop up” and occupy more space only when “clicked” on. What I really liked was also the different arrangements the modals would take on different screen sizes.

Finally, I was not fully happy with the iframe images I got from youtube. I wanted to add a little bit of “movement” to the videos and the page as a whole. After all, we’re talking about a particular type of music which, to this day, still makes people want to boogie. This led me to decide that I wanted to use gifs rather than still images for my video placeholders.

Rather than creating the GIFs myself, I was introduced to the “new-ish” animated thumbnail feature from Youtube. The “moving thumbnails are automatically generated with AI from a clip from the first half of the video that “it believes gives the best idea of what your video is about” ”.
I was very fond of the idea of incorporating some AI-like feature into this simple website, and that is why I decided to continue with this.
https://www.theverge.com/2017/7/14/15973058/youtube-gif-thumbnails-video-previews-why-is-it-moving

General layout

For the general look of the page, I just used a simple Bootstrap one-page template as I thought this would be enough to showcase all of the features I wanted to include without adding any complications to the overall UX. I used a simple template that I had made a few months back, for an experiment, as it seemed to suit this exercise.

When it came to making a decision on the overall color palette for the website, I went to a website called color-hex.com looking for a palette that would give a 1960s vibe to the website. I opted for the “Retro Color Palette” (https://www.color-hex.com/color-palette/165) as I especially liked its “yellow and red-like” colours. 

Main Image

For the website’s main image, I decided to use the cover from the Monkees’ Classic Album Collection and then edited the image slightly in Photoshop to give it a retro/cartoon-like effect. This turned out to work nicely with the overall color palette. In order to get the desired effect, I loosely followed the instructions from the video below as well as my own (6+ years) experience with Photoshop
https://www.youtube.com/watch?v=Qi6-H5KgKEE

Contact form
I finally built a working HTML contact form using a Bootstrap 4 framework and AJAX with PHP. For this feature,  I followed a tutorial from Bootstrapious which allowed me how to code the contact form in HTML, and add real-time validation to any required fields. I then followed their instructions to code the PHP script which handles the data in the contact form and sends the email to the intended recipient. Lastly, I used JQuery to submit the form via AJAX.

Tutorial link below:
https://bootstrapious.com/p/how-to-build-a-working-bootstrap-contact-form

Technologies Used:

JQuery
The project uses JQuery for a number of different purposes: for the Youtube videos within modals feature, for the validation of the contact form and its sending via AJAX

Javascript
The project uses Javascript for a number of different purposes: for playing the MP3 files from the “Jukebox” and for some Bootstrap features to work

PHP
The project uses PHP to handle email sending

Testing

In this section, I show tests of the user stories as outlined in the UX section. I also try to talk about how different elements of the website look and work on different browsers and screen sizes.

-> As an older fan of the Monkees, I’d like to re-listen to their greatest hits so that my mind may travel back to those days:
-Go to the main page
-Hover over “Jukebox” on the nav bar or the “Our Jukebox” button, these should react when hovered over
-Click on either of them and be taken to the Jukebox feature which is located a few sections down on the same page
-Click on any of the vinyls’ play buttons and that specific track should automatically start playing in the background.
-Once clicked on, the song should start playing and the writing on the button should now say “stop”. 
-Click it once again, to stop the track.

-> As a soon-to-be wife/husband , I’d like to try and book the Monkees to play at my wedding ceremony
-Go to the main page
-Hover over “Contact” on the nav bar or the “Contact us” button, these should react when hovered over
-Click on either of them and be taken to the Contact form which is located as the last section on the same page
-Fill all the required fields and select “wedding” as the event type for which you are contacting the Monkees
-Submit the form and verify that a success message appears


-> Testing the Monkees contact form
-Go to the contact form section by clicking on “Contact us” or scrolling to the bottom of the page
-Try to submit the empty form and verify that an error message about the required fields appears
-Try to submit the form with an invalid email address and verify that a relevant error message appears
-Try to submit the form with all inputs valid and verify that a success message appears.

Designing a responsive website:
Having mainly dealt with Bootstrap elements, it was expected that these would be automatically responsive to the browser size. Therefore,there wasn’t much work involved in making most of these elements look “good” on different screens.

With what regards to the Jukebox, however, I noticed that the linear arrangement of the vinyls would not work on screens that were smaller than 991px (tablets and mobiles). This is because the disks would get pushed one on top of the other, making it almost impossible to select a track. I therefore had to use CSS media queries and the display:none property as well as including a carousel item that only appears on smaller screens. 

The final result is that on tablets and mobiles, when you scroll down to the Jukebox feature, you can see a single record which can be played and stopped as normal. In order to “flick” through the stack of vinyls, the user needs to click on the left and right arrows which appear on the side of the record.

Deployment
I decided to opt for a very simple deployment to Github pages.
The website can be accessed via the link below:                    https://asi9games.github.io/TheMonkees/
