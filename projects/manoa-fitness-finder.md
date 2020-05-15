---
layout: project
type: project
published: true
image: images/logo.png
title: Manoa Fitness Finder
permalink: projects/manoa-fitness-finder
# All dates must be YYYY-MM-DD format!
date: 2020-05-13
labels:
  - IntelliJ IDEA
  - JavaScript
  - CSS/Html
summary: Creating a website for UH Manoa campus students to schedule and meet up for events.
---

Take a look at the source code for the project <a href="https://github.com/manoafitnessfinder">here</a>.

## Finding Friends

Its your first semester on a new campus and you are wanting to put yourself out there but you still haven't really met anyone yet. How would you get together with enough people to play a game of basketball? Enter Manoa Fitness Finder. The goal of the site is allow you post events that all your fitness friends can see and then to allow them to say I'll see you there without having to start a giant group text each time. It also allows you to add other people who share similar interests and see what events they having that are coming up.

 <div style="text-align: center">
    <img src="../images/manoa-home-page.PNG" alt = ''> 
 </div>

## My Role

My role for this project was project manager. My group, being one of the larger groups, quickly realized that if we were going to do this all remotely (thanks COVID-19) then a lot of coordination needed to be done to ensure that we didn't step on each others toes. My primary tasks included: using github project boards to update all tasks currently being worked on, identify new issues and assign them, presentations, as well as updating the team on the progress of site and upcoming deadlines. In addition I assisted with smaller features that were technologically challenging or with challenges that individual group members were having.
 
 
## Learn by Reviewing rather than by Doing
 
 Being a project manager I was in charge of doing the testing of the pages and features as they would get implemented. This meant that I had to quickly test all included functionality and then see what could be easily expanded or added to add more functionality to the site. This is what also what allowed me to learn. 
 
 By seeing the way someone else tackled, or was trying to tackle, a problem it gave me a better understanding of how the problem could be solved. From this I was able to learn many different ways to accomplish the same task. However sometimes the new tech can be a bit too much. This is tale of how  components are good thing but can make things more complicated if too many are used. 
 
 ### The tales of Components
 
 It started out easy. The profile page displays the comments the other users have left on your profile at the bottom of the page. Rather add the notes to the Profile collection a separate collection was made to store the notes with a link being the user's email address so they could be displayed in the page. Then the profile page was made to handle the the displaying of the notes on the page. This was changed to model it after the My events page.
 
 In the My events page. A collection was also made to store the events with the link being the users email address as the owner. This page was instead built with a component for the individual events. When a new event was made it was added in the my event page but the event was handed off the event component to be rendered on the page. This ended up being the correct choice as the events were displayed on other pages on the site. So, rather than having to copy and paste the code needed to render the events they could be sent to the event component to be rendered.
 
 This is were things got a little crazy. After making the events then we wanted to allow users to subscribe to events to say that they would be attending the event to expect to see them. So rather than extending the events collection another collection was made called attending to display the users, but rather then send the info to the events component it had its own component that would render the attendees on the event card. See the diagram below if you are confused:


 <div style="text-align: center">
    <img src="../images/event%20page.PNG" alt = ''> 
 </div>
 
 This ended making editing the attending events a nightmare. In end the events collection should had been expanded with the attending list because they are always displayed together. 