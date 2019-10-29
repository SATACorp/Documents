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
* The content displayed within the main user feed
* Content displayed by the quizzes
* Leaderboard with point totals for top 3 users + current user
* User Profile
### Controllers
* Navigation buttons displayed on the Navbar
* Buttons displayed on quiz
* Login button
* Back arrows (to exit a quiz, exit out of a user profile that you've tapped on) 

### Method Stubs
* Quiz model retrieves a quiz's questions and answers
   1. Pre-condition: Quiz exists, quiz has both questions and corresponding answers that aren't "NA"
   2. Post-condition: Returns the answers
  
  public static Answer retrieval (List quizzes, Quiz quiz) {
     if (!quizzes.contains(quiz)) { 
        return "this doesn't work" 
     } else {
        return quiz.Answers;
     }
  }
  
* Quiz model takes in answers and compares those answers with the right answers that are stored in the backend and returns the results of that comparison
   1. Pre-condition: Gets the answers from the retrieval method
   2. Post-condition: Returns results based on an internal comparison between user's answers and the right answers that are stored, returns count of right answers
   
public static int countOfRightAndWrongAnswers(String userAnswer) {
   List answers = retrieval(quizzes, quiz);
   int countRight = 0;
   int countWrong = 0;
   for (String answer : quiz.Answers) {
      if (answer.equals(userAnswer)) {
         countRight++;
      }
   }
   return countRight * 100;
}

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




  





