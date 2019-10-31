## Architecture
### Models
1. QuizModel
  * This component is a Model that stores all the quizzes that can be shown to the user and the results of each quiz that the user has submitted 
  * This component is only stored on the server 
  * The QuizController communicates with this Model 
    1. QuizController asks QuizModel to retrieve questions from the quiz 
    2. QuizController asks QuizModel to retrieve results from the quiz (if the given answers are correct or not)
    3. QuizController asks QuizModel to update user points and the given answers to a quiz for each user


2. LeaderboardModel
  * This component is a Model that contains all the points for every user on the platform. It allows for users to see the top people on the leaderboard, their points, and how the current user stands compared to them 
  * this component is stored on the server, but it is called upon and kept in the memory on the client side
  * The LeaderboardController communicates with the Model
    1. LeaderboardController asks LeaderboardModel to retrieve the points and users from the server 
    
3. UserModel
  * This component is a Model that contains all the relevant information about the user, including the user id, quiz points, list of articles read, and photo feed.
  * this component is stored on the server, but it is called upon and kept in the memory on the client side
  * The UserController communicates with the Model
    1. UserController asks UserModel to retrieve the user information from the server
    
4. LoginModel
  * This component is a Model that communicates with the Instagram API to allow users to login to their Instagram using a third party application 
  * Users interact with this model on the client side but the server sides hosts all the user's data via Instagram.
  * The LoginController communicates with this Model
    1. LoginController asks LoginModel to log the user in to the application given the right username and password 
    
    
### Views
1. The content displayed within the main user feed
   * The main user feed will replicate that of Instagram's with recent posts from the user's followings in a scrollable fashion. After every 10th post that appears on the feed, there will be a clearly defined news post with a short summary of the information in the article. Users will have the option to click on the article to go to another website with the full story. 
2. Content displayed by the quizzes
   * The quizzes view will contain available quizzes that the user can click on and take. Once a quiz is selected by the user, they will be prompted to answer questions based on that article, and will press "Submit." Upon completion of the quiz, the app will redirect to the initial quiz screen where they selected a quiz.  
3. Leaderboard with point totals for top 3 users + current user
   * The leaderboard view will contain a list of the top 3 application user's names and their scores, as well as accompanied by the current user's point total on the bottom of the screen. If the user is one of the top 3 users, then the last place user will have their points total be on the bottom of the screen. 
4. User Profile
   * The user profile view will include the user's name, number of followers, number of followings, and posts that they've made.

### Controllers
* Navigation buttons displayed on the Navbar
   1. Username/icon of poster
   2. "Go To Article" button
   3. Caption expander
   4. Profile pics thumbnail
* Buttons displayed on quiz
   1. Answer buttons
   2. Submit button
   3. Quiz icon
* Login button
* Back arrows
   1. To exit a quiz
   2. Exit out of a user profile that has been tapped/clicked on

### Method Stubs
* Quiz model retrieves a quiz's questions and answers
   1. Pre-condition: Quiz exists, quiz has both questions and corresponding answers that aren't "NA"
   2. Post-condition: Returns the answers
  
* Quiz model takes in answers and compares those answers with the right answers that are stored in the backend and returns the results of that comparison
   1. Pre-condition: Gets the answers from the retrieval method
   2. Post-condition: Returns results based on an internal comparison between user's answers and the right answers that are stored, returns count of right answers

* Quiz model updates the users points
   1. Pre-condition: User exists, user's point value is greater than or equal to 0, gets values from the comparison method 
   2. Post-condition: Increments user's point total based on the returned value from comparison method
   
* Leaderboard model retrieves and sorts the top 3 highest scoring users and shows the user's leaderboard if not in the top 3 
   1. Pre-condition: 1 or more users exist 
   2. Post-condition: Sorts and displays top 3 users highest to lowest, keeping in account the user's score. If user is not a part of top 3 users, their ranking is displayed underneath the leaderboard with their points total. 

* User model retrieves a user's information from the server
   1. Pre-condition: user exists and has a valid id
   2. Post-condition: returns user's personal data (id, points, articles read, feed)

* Login model communicates with the Instagram API to login the user and retrieve Instagram information
   1. Pre-condition: valid username and password is entered (user exists)
   2. Post-condition: retrieves user information, valid API usage
   
   
 ###  Link to Source Code with code stubs: https://github.com/SATACorp/Application





  





