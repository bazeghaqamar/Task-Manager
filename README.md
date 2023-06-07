# Task-Manager
Task given to alter code to reflect certain capabilities within it to manage tasks!

Instructions given:

Use the task_manager.py file for this project. Also, make use of the supporting text files (user.txt and tasks.txt) that accompany this Capstone project in this folder. In this task you will be modifying this program.

You will notice that the main body of the code requires functionality for registering a user, adding a task, viewing all tasks and viewing the current user's tasks. However, because there is so much functionality needed to complete this, the main body of the loop becomes difficult to read. Using the principle of abstraction, refactor the code to create and use the following functions:
- reg_user - called when the user selects 'r'
- add_task - called when a user selects 'a' to add a new task
- view_all - called when users type 'va' to view all the tasks listed in 'tasks.txt'
- view_mine - called when users type 'vm' to view all the tasks that have been assigned to them


Modify the function called reg_user to make sure that you odn't duplicate usernames wehn you add a new user to user.txt. If a user tries to add a username that already exists in user.txt, provide a relevant error message and allow them to try to add a user with a different username.


Add the following functionality when the user selects 'vm' to view all the tasks addigned to them:
- Display all tasks in a manner that is easy to read. Make sure that each task is displayed with a corresponding number which can be used to identify the task. 
- Allow the user to select either a specific task (by entering a number) or input '-1' to return to the main menu.
- If the user selects a specific task, they should be able to choose to either mark the task a complete or edit the task. If the user chooses to mark a task as complete, the 'Yes/No' value that describes whether the task has been completed or not should be changed to 'Yes'. When the user chooses to edit a task, the username of the person to whom the task is assigned or the due date of the task can be edited. The task can only be edited if it has not yet been completed. 


Add an option to generate reports to the main menu of the applications.

When the user chooses to generate reports two text files should be generated. Both these text files should output data in a user-friendly, easy to read manner. 


Task_overivew.txt should contain:
- Total number of tasks generated and tracked
- Total number of completed tasks
- Total number of uncompleted tasks
- Total number of tasks that haven't been completed and are overdue
- Percentage of tasks that are incomplete
- Percentage of tasks that are overdue


User_overview.txt should contain:
- Total number of users registered with task_manager.py
- Total number of tasks that have been generated and tracked using task_manager.py
- For each user also describe:
  - Total number of tasks assigned to that user
  - Percetange of total number of tasks that have been assigned to that user
  - Percentage of the tasks assigned to that user that have been completed
  - Percentage of the tasks assigned to that user that must still be completed
  - Percentage of the tasks assigned to that user that have not yet been completed and are overdue


Modify the menu option that allows the admin to display statistics so that the reports generated are read from tasks.txt and user.txt and displayed on the screen in a user-friendly manner. If these text files don't exist, first call the code to generate the text files. 
