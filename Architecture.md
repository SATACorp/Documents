## Architecture
### Models
* Supported by an external online server, the data will reside mostly outside of the application.
* State management handled within contextually within Main application component. Smaller components will be stateless
### Views
* The content displayed within the main user feed
* Content displayed by the quizzes
### Controllers
* Navigation buttons displayed on the Navbar
* Buttons displayed on quiz

<ol>QuizModel
  <li> This component is a Model that stores all the quizzes that can be shown to the user and the results of each quiz that the user has submitted </li>
  <li> This component is only stored on the server </li>
  <ol> The QuizController communicates with this Model 
    <li> QuizController asks QuizModel to retrieve questions from the quiz </li>
    <li> QuizController asks QuizModel to retrieve results from the quiz (if the given answers are correct or not) </li>
    <li> QuizController asks QuizModel to update user points and the given answers to a quiz for each user </li>
  </ol>
<ol>LeaderboardModel
  <li> This component is a Model that contains all the points for every user on the platform. It allows for users to see the top people on the leaderboard, their points, and how the current user stands compared to them </li>
  <li> this component is stored on the server, but it is called upon and kept in the memory on the client side </li>
  <ol> The LeaderboardController communicates with the Model
    <li> LeaderboardController asks LeaderboardModel to retrieve the points and users from the server </li>
  </ol>
</ol>



