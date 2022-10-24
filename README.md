# KeyUA test task

### Description
Your goal is to write a simple peer-to-peer chat application.

### Domain (business logic) requirements
1. The user should be able to create a profile with username + password, login & logout
1. The user should be able to upload an avatar & have it displayed in chats
1. The user should be able to create a chat
1. The user should be able to manage a chat - add/remove members or change it's name
1. The user should be able to delete a chat
1. The user should be able to send message to an available chat
1. The user should be able to read messages from available chats
1. The user should be able to forward message from one available chat to another

### Tech requirements
1. Your application needs both site (Django) and a RESTful API (DRF) components. The latter is purposed for third-party apps
1. Site part should use session authentication, API part should use tokens
1. We need to keep file log of all requests, their path, execution time, and user ids
1. We need to keep a database log of all our models updates that will be accessible with admin interface

### Bonus tasks
You have a certain degree of freedom when it comes to making your application better. If you can think of any additional features or improvements that can show your competitive qualities - implement them. The only constraint limiting what you would want to add is that your features/improvements should be reasonable. Either from domain (business logic) or technical point of view. They also shouldn't be done instead of the requirements mentioned above, only in addition to them. If you can't think of any such tasks, here is a few:
1. Write a docker-compose setup for your application. It should consist of backend, database and web server (preferably [nginx](https://www.nginx.com/)) services plus anything you want to add in advance. Nginx should serve static & media content instead of backend service
1. Add unit tests for API and site views
1. Implement live updates to chats via web sockets (preferably using [channels](https://channels.readthedocs.io/en/stable/)) or polling (try to make it somewhat efficient)
1. Customize admin interface

### Important notes
1. You don't need to make a perfect commit history. Work at your own pace, commit at will
1. You don't need to make a design for a site, so don't bother with css. Use js within reasonable limits if you want
1. Utilize django/drf functionality as much as possible, no need to re-invent a wheel. If you want to include additional django packages/plugins be sure their use is justified. Such packages should not do any of the tasks mentioned above for you, but rather help you to do them
1. Try to write code in a concise and consistent manner. Writing good code is as important as meeting the domain and tech requirements. Also make sure the code meets basic pep8 requirements
1. Non-functional requirements also matter - security, performance, maintainability. Follow best practices and eliminate common mistakes as much as possible
1. To apply to the test fork this repository, write the code and replace README.md content with basic instructions to perform initial setup of your application
