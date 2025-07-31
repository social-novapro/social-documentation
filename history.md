# Version History
History of each update made to documentation.

Version numbers: <b>X.X.X (build.year.month.day)</b>

---
### 1.0 (15.2025.07.09) 
- Added onboarding section of documentation.

### 1.0 (14.2023.10.21)
- Rewrote every schema in /v1/schemas, was missing many, and had many outdated. |
- Started adding new/updated routes in /v1
- Updated main readme file
- added instructions to get started

---

### 1.0 (13.2022.11.13)
- added missing routes in /v1/readme.md, still need to write docs.
- added missing schemas (added in a new table).
- added version history.

---

### 1.0 (12.2022.07.26)
- Added new /v1/get routes from API.
- Completed /v1/get/bookmarks.
- Added new bookmarks schema.
- Added type in front of each schema type. (on main readme)
- Changed how numbering is done for api docs. Now each section has its own main number.
- Fixed /v1/get/user, it’s not a username param, but a userid param in required.

---

### 1.0 (11.2022.07.24)
- Added basic websocket docs.

---

### 1.0 (10.2022.07.03)
- Added corrected /v1/post/createPost/.
- Added updated /v1/delete/removePost/.

---

### 1.0 (9.2022.06.25) 
- Added userEdit to /v1 routes main page.

---

### 1.0 (8.2022.06.25) Merge pull request #3 from DumbGameMaker/patch-1
- Merged.

---

### 1.0 (7.2022.06.25) 
- Added new userEdit to documentation.
- Added to .gitignore.
- Updated userSchema.

---

### 1.0 (6.2022.06.24) Merge pull request #2 from DumbGameMaker/master
- Added errors to documentation.

---

### 1.0 (5.2022.06.24) Merge pull request #1 from DumbGameMaker/master
- Added post/requestVerify.
- Added descriptions for all endpoints.

---

### 1.0 (4.2022.05.03)
- Each route had headers example, but there was no commas in headers.
- Created documentation
    - /get
        - /allUsers
        - /analyticTrend
        - /post
        - /user
        - /search
        - /userByID
        - /userFeed (not done since code isn’t done)
        - /username
- In /v1 documentation, moved createPost to a Post section instead of Get section.

---

### 1.0 (3.2022.04.29)
- Main page now has a nice table for each version .
- /v1/readme.md now has a number for each route.
- Updated /v1/auth/checkToken and /v1/auth/userLogin with newer design from b2.
- Updated /v1/post/createPost has slightly updated look.

---

### 1.0 (2.2022.04.27)
- Fixed /v1/delete (was /v1/get) in v1/readme.
- Added a location area for the routes.
- Added 
    - V1
        - Delete
            - removePost
        - Get
            - allPosts
            - allPublicData
- New docs for routes each has JavaScript examples 
- Tried to activate GitHub pages. (on April 28th)

---

### 1.0 (1.2022.04.26)
- Created a project full of readme’s for the information about schemas and routes.
- Added files
    - readme.md
        - v1
            - readme.md
            - auth
                - checkToken
                - userLogin
            - Schemas
                - readme.md
                - developerAppToken
                - developerToken
                - interactPostSchema
                - interactUserAccessSchema
                - interactUserAnalyticSchema
                - interactUserSchema
