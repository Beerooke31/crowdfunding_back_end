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

| URL | HTTP Method | Purpose | Request Body | Success Response Code | Authentication/Authorisation |
| /projects/ | GET | Returns all projects | N/A | 200 | N/A |
| /pledges/ | GET | Returns all pledges | N/A | 200 | N/A |
| /users/ | GET | Returns a list of all users | 200 | Must be admin?|
| /projects/ | POST | Creates a new project | 201 | Must be logged in |
| /pledges/ | POST | Creates a new pledge | 201 | Must be logged in |
| /users/ | POST | Creates a new user | 201 | Must be logged in |
| /projects/1/ | PUT | Updates project 1 | 200 | Must be logged in and project owner |

### DB Schema

![]( {{ ./relative/path/to/your/schema/image.png }} )
