# Crowdfunding Back End

Brooke Pierson

## Planning:

### Concept/Name

Starbounty - A crowdfunding platform to fund occult research. This could include endeavours such as exploration of a haunted house or a UFO crash landing site, with researchers ranging from scientists to your average Joe. Project creators can gain funding for tools, travel expenses, amenities - basically anything they require to conduct their research and unravel the mysteries of the universe.

### Intended Audience/User Stories

The intended audience/user includes researchers interested in occult studies who want to create a crowdfunding campaign to allow access to the necessary resources to investigate their chosen topic.
A secondary user is someone who has a desire to know more about paranormal topics but doesn't necessarily want to go out into the field themself, however, is happy to donate to an individual/group who can investigate on their behalf and provide feedback on their findings.

### Front End Pages/Functionality

- {{ A page on the front end }}
  - {{ A list of dot-points showing functionality is available on this page }}
  - {{ etc }}
  - {{ etc }}
- {{ A second page available on the front end }}
  - {{ Another list of dot-points showing functionality }}
  - {{ etc }}

### API Spec

| URL              | HTTP Method | Purpose                               | Request Body                                                                                                                                                                                                                                                   | Success Response Code | Authentication/Authorisation    |
| ---------------- | ----------- | ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- | ------------------------------- |
| /api-token-auth/ | POST        | Returns authentication token for user | {<br>"token": "",<br> "user_id": "",<br> "email": ""<br>}                                                                                                                                                                                                      | 200                   | N/A                             |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /projects/       | GET         | Returns all projects                  | N/A                                                                                                                                                                                                                                                            | 200                   | N/A                             |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /projects/1/     | GET         | Returns a project with ID "1"         | N/A                                                                                                                                                                                                                                                            | 200                   | N/A                             |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /projects/       | POST        | Creates a new project                 | {<br>"title": "",<br> "description": "",<br> "goal": "",<br> "image": "",<br> "is_open": "",<br>"date_created": ""<br>}                                                                                                                                        | 201                   | Must be logged in               |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /projects/1/     | PUT         | Updates project with ID "1"           | {<br>"title": "",<br> "description": "",<br> "goal": "",<br> "image": "",<br> "is_open": "",<br>"date_created": ""<br>}                                                                                                                                        | 200                   | Must be logged in.              |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       | Must be project owner or admin. |
| /projects/1/     | DELETE      | Deletes project with ID "1"           | N/A                                                                                                                                                                                                                                                            | 204                   | Must be logged in.              |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       | Must be project owner or admin. |
| /pledges/        | GET         | Returns all pledges                   | N/A                                                                                                                                                                                                                                                            | 200                   | N/A                             |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /pledges/1/      | GET         | Returns a pledge with ID "1"          | N/A                                                                                                                                                                                                                                                            | 200                   | N/A                             |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /pledges/        | POST        | Creates a new pledge                  | {<br>"id": "", <br>"supporter": "",<br> "amount": "",<br> "comment": "",<br> "anonymous": "",<br> "project": ""<br>}                                                                                                                                           | 201                   | Must be logged in.              |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /pledges/1/      | PUT         | Updates pledge with ID "1"            | {<br>"id": "",<br> "supporter": "",<br> "amount": "",<br> "comment": "",<br> "anonymous": "",<br> "project": ""<br>}                                                                                                                                           | 200                   | Must be logged in.              |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       | Must be pledge owner or admin.  |
| /pledges/1/      | DELETE      | Deletes pledge with ID "1"            | N/A                                                                                                                                                                                                                                                            | 204                   | Must be logged in.              |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       | Must be pledge owner or admin.  |
| /users/          | GET         | Returns a list of all users           | N/A                                                                                                                                                                                                                                                            | 200                   | N/A                             |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /users/1/        | GET         | Returns user with ID "1"              | N/A                                                                                                                                                                                                                                                            | 200                   | N/A                             |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
| /users/          | POST        | Creates a new user                    | {<br>"id": "",<br> "last_login": "",<br> "is_superuser": "",<br> "username": "",<br> "first_name": "",<br> "last_name": "",<br> "email": "",<br> "password": "",<br> "is_active": "",<br> "date_joined": "",<br> "groups": "",<br> "user_permissions": ""<br>} | 201                   | Must be logged in.              |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |
|                  |             |                                       |                                                                                                                                                                                                                                                                |                       |                                 |

### DB Schema

[ERD_Diagram](./Crowdfunding_ERD.png)

### Link to deployed project

https://starbounty-d5b76e766824.herokuapp.com/

### Insomnia Screenshots

[Insomnia Screenshots](./screenshots)

### User and Project Registration Steps

[User Steps](./User_Steps.png)

[Project Steps](./Project_Steps.png)
