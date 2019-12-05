## Requirements: 

By: Anant Rajeev, Thomas Penner, Chris Forbes, Amogh Dave, Sanjay Unni

* The app will have a consistent user experience by following the same design choices as the original Instagram app; our app will use the same typefaces, buttons, margins, shapes, icons, color palettes, text boxes, and other elements of visual design in all parts of the app.
        <br/>   Complete
        Revised: our app is no longer connected to Instagram so it relies on its own custom-made design, but said design is consistent throughout
* When the InstaNews web app is opened, the initial login page will be presented.
    -Complete
* The login page will utilize Instagram’s login user interface through the Instagram API, in which the user will be able to login through Facebook or through their Instagram username and password.
    -Complete
    -Revised: our app is no longer connected to Instagram, but has a login/signup interface that relies on a user-made username and password
* On mobile, the navigation bar will be fixed at the bottom of the web page, taking up the width of the screen. On larger screens such as desktops, the navigation bar will be at the top of the screen and take up the width.
    -Complete
    -Revised: there were no functional changes by moving the navbar (did not change the scope or inherent functionality of the app) and it was easier to code/design with it at the bottom, so we have it moved to the bottom of the screen on all devices
*  The navigation bar will have four navigation buttons. From left to right in evenly spaced buttons: Main feed, quizzes, leaderboard and profile.
    -Complete
* The website will be mobile optimized, which means it will be designed to work for the screen size of a phone. However, it will also work with larger screens by increasing the amount of blank space on the sides. This can be done using media queries.
    -Complete
* The quizzes page will contain quizzes about the latest news articles. There will be 3 questions per quiz. Each correct answers will award the user with 10 points.
    -Complete
* Quizzes will consist of multiple choice questions and true/false questions. Multiple choice questions will have four answer options, labeled alphabetically from ‘A’ to ‘D’.
    -Complete
    -Revised: in the process of making quizzes we found that we already had pre-made multiple chioce bubbles, so alphabetical lettering was not necessary (additionally, we already randomize answer choices so ordering them would not matter)
* The feed will include photos from the user’s Instagram followings interspersed with news clippings which will include a headline, and a small summary of the article. These news posts will appear after every 5 posts from a user’s normal feed. 
    -Complete
    -Revised: our app is no longer connected to Instagram so anything pertaining to data (i.e. photos) from it no longer stands, but the part about the news clippings is still relevant so we have met that part of the requirement.
* The likes and comments of a photo will show up underneath a photo in a separate screen after a user double taps or double clicks on that photo in the feed; the photo alone will be shown with that user’s username and a back arrow will be shown to allow users to go back to the feed. On news posts, likes and comments are not directly shown. Instead, double clicking/tapping on the news post redirects to the news article. 
    -Complete
    -Revised: our app is no longer connected to Instagram so we no longer show photo data (username, likes, comments) but we have kept the ability to go to the news article from the news post (which we simplified into a "read article" button)
* An external web page will open once the user double taps or double clicks on the “Go to article” button next to a news feed.
    -Complete
* The user profile page will contain information about the user’s profile. It will show the username, the profile picture, and a grid view of the pictures the user has uploaded to Instagram in the past. It will also show the followers count, and following count of that particular user at the top of the screen.
    -Complete
    -Revised: our app is no longer connected to Instagram so it will not show Instagram user data but it does show our Firebase user data (username, profile picture, point count, leaderboard position)
* The leaderboard page will display the top three quiz point holders descending from the top; it will display how the user currently ranks against them. It will show profile pictures, numerical rankings of the quiz holders, and the point counts of those quiz holders along with the user.
    -Complete
* The system should be able to scroll infinitely downward to allow the user to see more news posts and images from the user's Instagram feed.
    -Complete
    -Revised: our app is no longer connected to Instagram so no Instagram posts (i.e. photos) show up in the feed, but news posts still do
* Interacting (clicking, tapping) on a username should redirect to that user's profile page within the InstaNews app.
    -Revised: after removing the connection to Instagram in our app, we felt like this was not a necessary addition to the app and therfore not something we absolutely had to have
* Interacting (clicking, tapping) on a news post will redirect the user to the external website with the full news article by opening up a new tab in the web browser and switch focus to that tab. 
    -Complete

