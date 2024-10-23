# crowdfunding_back_end

A repo to contain my SheCodes crowdfunding project

# Crowdfunding Back End

{{ Brooke Pierson }}

## Planning:

### Concept/Name

{{ Starbounty - A crowdfunding platform to fund occult research. For example, exploration of a haunted house or a UFO crash landing site. Researchers can post their projects and gain funding for their research, from tools they require to travel expenses. }}

### Intended Audience/User Stories

{{ My intended audience is anyone who is interested in learning more about the mysteries of this vast universe that we call home. It's for both people who want to actively seek answers and those who want the answers given to them. }}

### Front End Pages/Functionality

- {{ A page on the front end }}
  - {{ A list of dot-points showing functionality is available on this page }}
  - {{ etc }}
  - {{ etc }}
- {{ A second page available on the front end }}
  - {{ Another list of dot-points showing functionality }}
  - {{ etc }}

### API Spec

{{ Fill out the table below to define your endpoints. An example of what this might look like is shown at the bottom of the page.

It might look messy here in the PDF, but once it's rendered it looks very neat!

It can be helpful to keep the markdown preview open in VS Code so that you can see what you're typing more easily. }}

| URL          | HTTP Method | Purpose                       | Request Body         | Success Response Code               | Authentication/Authorisation              |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------------------- |
| /projects/   | GET         | Returns all projects          | N/A                  | 200                                 | N/A                                       |
| -----------  | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------              |
| /projects/1/ | GET         | Returns a project with ID "1" | N/A                  | 200                                 | N/A                                       |
| -----------  | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------              |
| /projects/   | POST        | Creates a new project         | Created              | 201                                 | Must be logged in                         |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------              |
| /projects/1/ | PUT         | Updates project with ID "1"   | Successful           | 200                                 | Must be logged in. Must be project owner. |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------              |
| /pledges/    | GET         | Returns all pledges           | N/A                  | 200                                 | Must be logged in.                        |
|              |             |                               |                      |                                     | Must be project owner.                    |
| -----------  | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------              |
| /pledges/1/  | GET         | Returns a pledge with ID "1"  | N/A                  | 200                                 | N/A                                       |
| -----------  | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------              |
| /pledges/    | POST        | Creates a new pledge          | Created              | 201                                 | Must be logged in.                        |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------              |
| /pledges/1/  | PUT         | Updates pledge with ID "1"    | Successful           | 200                                 | Must be logged in. Must be pledge owner.  |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------------------- |
| /users/      | GET         | Returns a list of all users   | N/A                  | 200                                 | Must be admin.                            |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------------------- |
| /users/1/    | GET         | Returns user with ID "1"      | N/A                  | 200                                 | Must be admin.                            |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------------------- |
| /users/      | POST        | Creates a new user            | Created              | 201                                 | Must be logged in.                        |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------------------- |
| /user/1/     | PUT         | Updates user with "1" details | Successful           | 200                                 | Must be logged in.                        |
| ------------ | ----------- | ----------------------------- | -------------------- | ----------------------------------- | ----------------------------------------- |

### DB Schema

![]( {{ ./relative/path/to/your/schema/image.png }} )
