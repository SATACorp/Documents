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

1. QuizModel
  * This component is a Model that stores all the quizzes that can be shown to the user and the results of each quiz that the user has submitted 
  * This component is only stored on the server 
  * The QuizController communicates with this Model 
    1. QuizController asks QuizModel to retrieve questions from the quiz 
    2. QuizController asks QuizModel to retrieve results from the quiz (if the given answers are correct or not)
    3. QuizController asks QuizModel to update user points and the given answers to a quiz for each user
2. LeaderboardModel
⋅⋅* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
⋅⋅1. Ordered sub-list
4. And another item.





