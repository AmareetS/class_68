# Topic: Wireless Library - Another case study

- Explore a case study of a wireless library management system for a low income school.
- Design a wireframe for the Wireless Library application. 
- Build tab navigation to issue/return and search for a book.

- Before, we start - one quick question. Does your school have a library?
- How are books managed in your library? 
- How do students issue/return books?
- How do students know which books are available, which are not and when they are going to be available?
- Who manages these books?
- Does your school have a librarian?
- User stories for Teacher reference:
  - As a teacher, I want to enter the student id, book id and submit the info so that I can issue the book to any student.
  - As a teacher, I want to enter the student id, book id and submit the info so that I can return the book issued by the student back to the library.
  - As a teacher, I want to be able to search for any book's availability in the library so that I can inform the students about the availability of any book.
  - As a teacher, I want to search for all the books issued by a particular student so that I can check for the books that were issued by the student.
- Now what will be the user flow of our app for a teacher in National Public School?
  - Any teacher who is free in a particular period can use the app to issue or return a book. Each book will have a unique id on it. Each student will also have a unique id. The teacher can enter this information (unique book id and student id) to issue the book to the student and store the information as an issued book. If the student has come up to return a book, the teacher will enter the same information (unique book id and student id) to return the book back to the library. The teacher can also search for a book by its id to check its availability in the library. The teacher can also search for books issued by any one particular student.

Each user story is a small,independently contained feature in an app which fulfills a user need. An app will have several user stories. A good user story goes like this: As a (<who is going to use the app>),I want to (<what action is the usergoing to take through the app>), so that (<what benefit will the user getout of the app>)If you observe, the user story answers the WHO, WHAT and WHY for an app feature you are going to build. This helps the developers and everyone involved in building the app bring more clarity as to what the app will do.

For example: One user story in our app will be: As a teacher, I want to enter the student id, book id and submit the info so that I can issue the book to any student.

- Do youremember what we did last time whenwe had to move between the twoscreens?How did we create the navigation?
  - We switched between twoscreens by pressing abutton.We used SwitchNavigator.Student reviews theSwitchNavigator.
  - explain how we created theSwitch navigation in our app.
    - We created twoscreens - BuzzerScreen and mainscreen
    - In app.js we createda switch Navigatorusing create SwitchNavigator. Itcontained twoscreens.
    - We created anAppContainercomponent using createAppContainer().
    - We then used theAppContainer in ourapplication.

- Creating a Tab Navigator isexactly the same!Let's start our app by creating asimple Tab Navigator which can helpus switch between the two screens -issue/return and search.