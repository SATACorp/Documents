# Design Specification

<h3>Roles:</h3>
- Anant Rajeev - CEO <br>
- Sanjay Unni - CDO <br>
- Chris Forbes - PM <br>
- Amogh Dave - CTO <br>
- Thomas Penner - CTO <br>

<h3>Mission Statement:</h3> Seamlessly integrating diverse news sources into social media to combat media illiteracy

<h3>Problem Statement:</h3> Instagram is currently one of the world's most popular social media platforms. Social Media (like Instagram) has arrested the attention of growing children, so much so that teens in today's world don't "have the time" to stay up to date on current events or pressing news matters. Despite the prevalence of cell phones and access to the Internet in the modern era, teenagers nowadays generally don't have the propensity for - or an interest in - keeping up with news sources and getting informed on current events. A general lack of knowledge about these important topics can slowly create an uninformed population. Ultimately, this population has to make decisions about the future of their society; poor choices can create cascading effects that can seriously impact future generations down the line. It's important to bring news and current events to prospective voters today, but in such a way that it becomes an everyday part of life rather than an intensive chore that's forced upon them. In doing so, teenagers can have the information they need to become productive members of society and set the standard for future generations to follow.

<h3>Solution:</h3> Our team envisions utilizing an Instagram API to recreate the application's feed, with the difference being that after a certain amount of photos and videos scrolled past, there is a snippet of a news story with a very short summary that they can quickly look at. 

<img src="./images/login.jpg" alt="login" width="280" height="500"> <img src="./images/feed.jpg" alt="feed" width="280" height="500"> <img src="./images/individualpost.jpg" alt="individual post" width="280" height="500">

<h3>Image Description: </h3>Users will log into the application using the same credentials they would on the Instagram app (IMG 1). Our service would use the Instagram API (as shown in the first image) to access the user's feed and relay it to them in a user friendly manner as shown in the second image. However, this feed would be modified to include "news posts" which are in the same format as as an Instagram post. The news post, as shown in the second image, will include a small blurb about the event/story and will include a "Go to Article" button in the top right corner that the user can click on to access an external website with the full article. The news events that are displayed are chosen using a backend web-scraping mechanism that picks up news stories from a variety of differing and reputed sources. The third image shows the event in which the user clicks or taps on an Instagram image post: the app will take the user into a display where they can see the amount of likes and comments, and the picture in its own tab. However, if the user clicks on one of the news posts, it will take them to the actual article so they can read further. 

<img src="./images/quiztab.jpg" alt="quiz tab" width="280" height="500"> <img src="./images/questions.jpg" alt="rewards" width="280" height="500"> <img src="./images/leaderboard.jpg" alt="leaderboard" width="280" height="500">


<h3>Image Description:</h3> As a method of analyzing success rate and seeing how well our application is fairing amongst our customers and how much they're learning, we intend to create a games/quizzes tab inside the application where users can go to take a quiz on what they've scrolled over. These quizzes are based on the news articles, found on the main feed, that the user has clicked or tapped on. In the game/quizzes tab (IMG 4), users can see the number of quizzes that're available and the number of quizzes they have completed. They can also see each quiz, the article it corresponds to, search through them by alphabetical order, and view the new or completed ones.

<img src="./images/userProfile.jpg" alt="user profile" width="280" height="500">

