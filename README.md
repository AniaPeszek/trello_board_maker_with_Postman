# Postman collection for creating monthly board
## The idea of Project
It is a simple Postman collection that creates month board in Trello, next it creates a list for each day with tasks according to the weekly schedule.
## Environment Configuration
- Import the environment.
- In edit window enter your `api-key` and `token`. Yuo can use the instruction from https://developer.atlassian.com/cloud/trello/guides/rest-api/api-introduction/
- Enter `monthNumber` (in range 1 to 12) to create the month table.
- Enter `currentDay` if you  don't want to start creating table since the first day of the month.
- You can change `year` if you want to.
- Enter `locales` eg. 'pl' or 'en'.

![image](environments.jpg?raw=true "environments")

## Creating month board
To create a board, firstly you have to provide your weekly schedule. Go to the first request:  get my boards and create task list variable. Then click on Pre-request Script. There you can enter your task for each weekday.

![image](task_list_data.jpg?raw=true "weeklyschedule")

Next, click on run the collection and uncheck the delete a board request in Collection Runner.

![image](collection_runner.jpg?raw=true "collection_runner")

Example monthly board

![image](example_board.jpg?raw=true "example_board")
