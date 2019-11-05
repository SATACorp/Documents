# Plan
 ## Coordination
  ### Roles
  * Thomas Penner and Amogh Dave (CTOs) will be in charge of delegating the technical componenets of our project to each member. The decisions will be made based on the the member's technical skill and the deadline on which the task or component must be completed.
  * Sanjay Unni (CDO) will be leading the design language of the app and will set deadlines for the iterative design components. He will also be in charge of any external vector design work and in delegating tasks for that.
  * Chris Forbes (PM) will make sure that everyone is on task and that the tasks are being completed. To do this, he will be communicating with the CTOs and CDOs to make sure all the delegated tasks can be completed in an efficient and reasonable time frame.
  * Anant Rajeev (CEO) will ensure consistency among the tech and design teams as well as assist in the development.

  Everyone has a key role in on our team. We laid out the roles accordingly so that everyone can be held accountable and will hold each other accountable for each other.

  ### Practices
  * We will be using Google Sheets to keep track of our tasks. Each task will be broken up by **component**, **task**, **assignee**, and a **rough deadline**. 
  * If deadlines are ever altered through the course of development, the deadline will be marked in red to signify an altered dealine. This is to ensure that everyone is aware that an assignee needed to make a necessary adjustment, and to hold him accountable for completing his task by the new deadline.

  Google Sheets is a very user friendly platform and we're all familiar with it. We all collectively agreed this will work best for our team in terms of assigning and acknowledging the completion of tasks.

  ### Weekly Meetings
  * We will take advantage of the class meetings to complete the bulk of our work. We will also be meeting at least once a week outside of class (~1.5-2 hours)

  ### Meeting Agenda
  * 10 -20 minutes on updates from each member
  * Reassignment of tasks as necessary
  * Reassignment of deadlines as necessary
  * Prioritizing tasks with respect to new deadlines
  * Developing components based on our priorities

  We are aware of everyone's busy schedules. This is why we want to take advantage of our class time to work on our project. We found it was also necessary to work on our project outside of class which is why we designated at least one outside class meeting where we can all meet. Any other small meeting decided among the members outside of our three required meetings are recommnended when needed, but optional.

 ## Communication
 * **Slack** will be used for primary discussing during our project
   * Alternatives: Text messaging, Facebook Messenger
   * Reason: We want to use a platform where we can keep our project discussions separate from other messaging platforms that we 
     use for personal use. This can help us in not being distracted during development. Slack also has integrations for sending         small snippets of code that can help us when we work remotely. We are also all familar with Slack.
 * **Google Sheets** will be used for documenting progress and completed components and tasks
   * Alternatives: Github Issues/Milestones, Trello
   * Reason: Again, all of us are familar with Google Sheets. While learning Github Issues and/or Trello may be beneficial for us       for industry standards, trying to learn how the platform works might slow down our progress.
  
 ## Ownership
 * **We will be utilizing the waterfall method.** We have one general overall plan with set deadlines for certain goals. Based on this, the CTOs will be assigning all the components to each member based on their technical skill and the deadline it needs to be completed by. The CDO may also assign any external design work if needed. As it stands right now, while we have a deeper understanding of our architecture, we do not know the difficulty in developing each component. We collectively agreed that we should **assign tasks as we go** so we can account for any last minute situations as well as develop a better understanding of each person's skill.

 ## Timeline
 * Everyone to finish the React tutorial from Scrimba.com as a refresher - **Deadline: 11/4**
 * Instagram API access to start working - this includes login portal, user profile, and photo feed imported into application interface - **Deadline: 11/12**
 * News API integrated into the system - this includes updating news aricles into a particular data structure and displaying that onto the application interface - **Deadline: 11/12**
 * Quiz page built with layout, appropriate quiz content, and proper backend score updating and reporting - **Deadline: 11/24**
 * Leaderboard section built with proper layout, displaying of the top 3 users, and the user's own score - **Deadline: 12/1**
 * Fine-tuning, problem solving, UX improvements, and small performance improvements - **Deadline: 12/5 RELEASE DATE**

 ## Verification
 * IF we make tests, they will cover our implementation of the Instagram API and the News API: ensuring the components concerned with this can call the APIs properly, grab information, manipulate that information with code, and display the desired information
 * IF there is a code inspection, because all of our components for the app are divided up, when one component in the app doesn’t render or stops working, that’s the component in the code that will be tested. 

   **Requirements and the Verification**
   * The app will have a consistent user experience by following the same design choices as the original Instagram app; our app will use the same typefaces, buttons, margins, shapes, icons, color palettes, text boxes, and other elements of visual design in all parts of the app.
     * Verification: A group review will be conducted to gauge if the user experience is smooth and user interface looks and feels up to par with our expectations. 
   * When the InstaNews web app is opened, the initial login page will be presented.
     * Verification:  There will be a manual test to see if the login box shows up on the webpage, this requirement will be validated if the box shows up and users are allowed to type inside the username and password fields.
   * The login page will utilize Instagram’s login user interface through the Instagram API, in which the user will be able to login through Facebook or through their Instagram username and password.
     * Verification: Once the user types in the username and password, and clicks on login, the landing page is shown with the user profile shown in the top right corner so the user can validate that the right profile was signed into. 
   * On mobile, the navigation bar will be fixed at the bottom of the web page, taking up the width of the screen. On larger screens such as desktops, the navigation bar will be at the top of the screen and take up the width.
     * Verification: This is a visual confirmation. If the navigation bar shows up at the bottom of the web page, and takes over the complete bottom of the screen (on cell phones) and at the top of the web page on desktops. 
   * The navigation bar will have four navigation buttons. From left to right in evenly spaced buttons: Main feed, quizzes, leaderboard and profile.
     * Verification: Visual confirmation. The navigation bar will have four logos symbolizing the buttons in the order shown above. 
   * The website will be mobile optimized, which means it will be designed to work for the screen size of a phone. However, it will also work with larger screens by increasing the amount of blank space on the sides. This can be done using media queries.
     * Verification: We will verify this through a manual test of the application, ensuring that each component behaves the same way on small and large screens. This will be done by a side by side comparison
   * The quizzes page will contain quizzes about the latest news articles. There will be 3 questions per quiz. Each correct answer will award the user with 10 points.
     * Verification: We will be writing Jest tests to confirm that our functions within the Quiz component successfully verify correct quiz answers, and administers points to the user successfully
   * Quizzes will consist of multiple choice questions and true/false questions.
     * Verification: Visual verification from the quiz module. Once a user clicks on a quiz, the quiz view shows up which shows the questions from the quiz, and four answer choices in the form of buttons with alphabetical labels. If these show up for quizzes, this requirement is validated
   * The feed will include photos from the user’s Instagram followings interspersed with news clippings which will include a headline, and a small summary of the article. These news posts will appear after every 5 posts from a user’s normal feed.
     * Verification: Also a visual verification. Upon login and the user is shown the modified feed, if the feed shows up and every 5th post is a news post that has a headline, picture, and a short summary, this requirement is validated. The news post has to be able to be clicked on and have it redirect to a new tab with the news 
   * The likes and comments of a photo will show up underneath a photo in a separate screen after a user double taps or double clicks on that photo in the feed; the photo alone will be shown with that user’s username and a back arrow will be shown to allow users to go back to the feed. On news posts, likes and comments are not directly shown. Instead, double clicking/tapping on the news post redirects to the news article.
     * Verification: We will manually test this by simply assessing if the likes and comments show up properly.
   * An external web page will open once the user double taps or double clicks on the “Go to article” button next to a news feed.
    * Verification: We will perform manual testing to confirm the functionality of the button. We will assess passes or fails based on the expected functionality of the button.
   * The user profile page will contain information about the user’s profile. It will show the username, the profile picture, and a grid view of the pictures the user has uploaded to Instagram in the past. It will also show the followers count, and following count of that particular user at the top of the screen.
     * Verification: This is a visual verification. Once the user logs in, the username and profile picture shows up in the top right. The pictures show up in an instagram like fashion. Once the user taps on the profile page, the page shows the followers count, and the following count. If these show up on the page, this requirement is validated. 
   * The leaderboard page will display the top three quiz point holders descending from the top; it will display how the user currently ranks against them. It will show profile pictures, numerical rankings of the quiz holders, and the point counts of those quiz holders along with the user.
     * Verification: Visual verification and backend verification - we will make sure that points are incrementing correctly after each quiz is taken and those points are updated in the leaderboard and the top 3 are shown in descending order. Backend verification is to make sure our sorting method is working and the user’s points are updating as quickly as possible. 
   * The system should be able to scroll infinitely downward to allow the user to see more news posts and images from the user's Instagram feed.
     * Verification: This will be a visual verification where we have a certain number of posts and elements rendered on a page and once the user scrolls past that number of posts/elements, then lazy loading will kick in and the next set of posts/elements will be rendered
   * Interacting (clicking, tapping) on a username should redirect to that user's profile page within the InstaNews app.
     * Verification: This will be a visual verification. If the user clicks on a username within the application, it should redirect to that user’s Instagram profile. 
   * Interacting (clicking, tapping) on a news post will redirect the user to the external website with the full news article by opening up a new tab in the web browser and switch focus to that tab.
     * Verification: This will be a visual verification - when a user taps/clicks on a news post that comes up in the feed, an external website should come up referring to that article
