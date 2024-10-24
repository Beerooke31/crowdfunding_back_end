# Crowdfunding Back End

Brooke Pierson

## Link to deployed project

https://starbounty-d5b76e766824.herokuapp.com/

## Planning:

### Concept/Name

Starbounty - A crowdfunding platform to fund occult research. For example, exploration of a haunted house or a UFO crash landing site. Researchers can post their projects and gain funding for their research, from tools they require to travel expenses.

### Intended Audience/User Stories

The intended audience/user includes researchers interested in occult studies, who want to create a crowdfunding campaign to fund their research project
so they can access the necessary resources to investigate their chosen topic.
A secondary user is an individual who doesn't necessarily want to seek answers about the mysteries of the universe themselves, but is happy to donate to a researcher who can investigate on their behalf.

### Front End Pages/Functionality

- {{ A page on the front end }}
  - {{ A list of dot-points showing functionality is available on this page }}
  - {{ etc }}
  - {{ etc }}
- {{ A second page available on the front end }}
  - {{ Another list of dot-points showing functionality }}
  - {{ etc }}

### API Spec

Fill out the table below to define your endpoints. An example of what this might look like is shown at the bottom of the page.

It might look messy here in the PDF, but once it's rendered it looks very neat!

It can be helpful to keep the markdown preview open in VS Code so that you can see what you're typing more easily.

| URL          | HTTP Method | Purpose                       | Request Body   | Success Response Code | Authentication/Authorisation      |
| ------------ | ----------- | ----------------------------- | -------------- | --------------------- | --------------------------------- |
| /projects/   | GET         | Returns all projects          | N/A            | 200                   | N/A                               |
|              |             |                               |                |                       |                                   |
| /projects/1/ | GET         | Returns a project with ID "1" | N/A            | 200                   | N/A                               |
|              |             |                               |                |                       |                                   |
| /projects/   | POST        | Creates a new project         | Project object | 201                   | Must be logged in                 |
|              |             |                               |                |                       |                                   |
| /projects/1/ | PUT         | Updates project with ID "1"   | Project object | 200                   | Must be logged in.                |
|              |             |                               |                |                       | Must be project owner.            |
| /projects/1/ | DELETE      | Deletes project with ID "1"   | N/A            | 204                   | Must be logged in.                |
|              |             |                               |                |                       | Must be project owner.            |
| /pledges/    | GET         | Returns all pledges           | N/A            | 200                   | Must be logged in.                |
|              |             |                               |                |                       |                                   |
| /pledges/1/  | GET         | Returns a pledge with ID "1"  | N/A            | 200                   | Must be logged in.                |
|              |             |                               |                |                       | Must be pledge owner.             |
| /pledges/    | POST        | Creates a new pledge          | Pledge object  | 201                   | Must be logged in.                |
|              |             |                               |                |                       | Must not be owner of the project. |
| /pledges/1/  | PUT         | Updates pledge with ID "1"    | Pledge object  | 200                   | Must be logged in.                |
|              |             |                               |                |                       | Must be pledge owner.             |
| /users/      | GET         | Returns a list of all users   | N/A            | 200                   | Must be logged in.                |
|              |             |                               |                |                       |                                   |
| /users/1/    | GET         | Returns user with ID "1"      | N/A            | 200                   | Must be logged in.                |
|              |             |                               |                |                       |                                   |
| /users/      | POST        | Creates a new user            | User object    | 201                   | Must be logged in.                |
|              |             |                               |                |                       |                                   |
| /user/1/     | PUT         | Updates user with "1" details | User object    | 200                   | Must be logged in.                |
|              |             |                               |                |                       |                                   |

### DB Schema

![x](./crowdfunding_back_end/Crowdfunding ERD.png)
