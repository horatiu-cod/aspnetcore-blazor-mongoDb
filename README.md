# Technical Advisor

Technical Supprt online App
Based on Blazor Server, Azure Active Directory B2C, MongoDB and Bootstrap 5

## App Skeleton

### App requirement questions:
* Do we want Authentification/Authorization?
* Do we want to limit what question a person can ask? Rate limit?
* Offensive content filter
* Should we show off a user's contribution?
* How the system knows if I have voted on a question?
* Should we limit the size of questions/description?
* Can we add new categories/ststuses?
* How do admin add status to a question?
* What happens when the list gets huge?

### Version 1 Features:
* Authentification/Authorization
* Approve/Deny questions as admin
* Admin Approval Screen
* Login/Account/Logout options
* User Profile Page
* Track the user's votes
* Limit the size of the title and description
* Admin to add categories
* Admin to add a status toa question with a note
* Admin feature for archiving questions

### App Major Components
* Blazor Server
* Azure Active Directory B2C (Authentification/Authorization)
* MongoDB (Database)
* Virtualize (Lazy Load)
* In-Memory Caching (scalability)
* Bootstrap 5

### App Data Design
* Category:
- CategoryName
- CategoryDescription

* Status:
- StatusName
- StatusDescription

* User:
- ObjectId  (Azure active directory id)
- FirstName
- LastName
- DisplayName
- EmailAddres
- AuthoredQuestion
- VotedOnQuestion

* Question:
- Question
- Description
- DateCreated
- Category
- Author
- UserVotes
- QuestionStatus
- OwnerNotes
- ApprovedForRelease
- Rejected
- Archived
 




