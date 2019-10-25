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

1) QuizModel
*  This component is a Model that stores all the quizzes that can be shown to the user and the results of each quiz that the user has submitted 
* This component is only stored on the server
* The QuizController communicates with this Model  

