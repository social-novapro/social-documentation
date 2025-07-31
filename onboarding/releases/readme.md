## Pre-Release and Release Process 
Last Updated, July 30, 2025

This document outlines the process for managing pre-releases and releases for any repostory in the Interact  project. It includes guidelines for feature development, pull requests, versioning, and release notes.

### Per feature Git
1.  Once each feature is complete, developer should create a pull request to the `dev` branch. 
2.  The pull request should be reviewed by at least one other developer.
3. After approval, the pull request can be merged into the `dev` branch.
4. The commit message for the PR should include the version number, build, date, and the feature name.
  - Format: `Major.Minor[.Patch] (Build.Year.Month.Day) - Feature Name`
  - Example: `1.9.1 (120.2025.07.30) - Feature Name`
  - Date should be in the format (YYYY.MM.DD) listed after the build number.
  - Any fixes will be incremented the next patch version number not released. X.X.X
  - Any new features will be incremented with the next minor version number not released. X.X 
5. Once merged, the developer should prepare a update note in the featue issue. 
- Any changes, including bug fixes, and new features should be noted in 3-8 bullet points. 
- Developer should include the number and name of the issue as the last bullet. 
- Example: `- 210 - New Explore Page`
6. The developer should mark the issue as complete and close the issue.

### Pre-release Git
1. Once all features are ready for the next release, project manager should create a new pull request to the `master` branch.
2. The pull request should be reviewed by at least one other developer.
3. After approval, the pull request can be merged into the `master` branch.
4. The commit message for the PR should include the version number, build, date, and the release name.
  - Format: `Major.Minor[.Patch] (Build.Year.Month.Day) - v.Major.Minor[.Patch] Release`
  - Example: `1.9.1 (120.2025.07.30) - v1.9.1 Release`
  - Date should be in the format (YYYY.MM.DD) listed after the build number.
5. Every new feature and bug fix should be documented in the PR for the release.
- 3-8 bullet points the release should be noted in the PR.
- Project manager should include the number of new commits, and the number of lines added/removed in the entire release.
- Example: `+15 Commits, +444/-83 lines`
6. Once merged, the project manager should create a new release in GitHub.

### Release Notes Git
1. The project manager should open releases in GitHub and draft a new release.
2. Select a new tag. and type in the version number of the latest commit in the `master` branch. Then select `Create new tag: v(version number)`.
- Example: `v1.9.1`, `v1.9.0`
3. Target the `master` branch for the release.
4. Release title should be the same as the tag name. 
- Example: `v1.9.1`, `v1.9.0`
5. Now start to write the release notes. This should include sections for:
- Release title, Information, Basic {x->z} Updates, Details {x->z} Updates, and Automated Release Notes. Please check out the [Example](#Example-Release-Notes).
   - Where x->z is which reposities have been updated for the current release, mainly for minor updates, patches most likely will not include more than one repository.


### Future Changes
- The process may be updated in the future to include automated release notes generation.
   - Hopefully using a script to geneate release notes from issues and pull requests.
- Every feature should not have the verison number in the commit message, only the dev->master PRs should have the version number.
- Will keep build number and date in the commit message for future reference.



### Example Release Notes
```
# Release v1.9.0
July 24, 2025

# Information

This is the v1.9 official release of Interact, Nova Production’s Social Media Platform, created by Daniel Kravec.

Find interact's information website: https://novapro.net/interact/

Check out interact: https://interact.novapro.net/

### Basic Frontend Updates
- New Explore Page
- Redesigned Settings Page
- Redesigned Menu Actions

### Basic Backend Updates
- Personalization Feed working
- New explore route in search 
- Bug fixes

### Detailed Updates, frontend

1.9 (153.2025.07.24) - UI Improvements
- Created a new explore page when selecting search
- Redesigned Settings Page with categories
- Redesigned Menu Action context
- 150 UI improvements

v1.9 (154.2025.07.24) - v1.9 Release
- Personalized Feed is now working
- New explore page for search
- Redesigned Settings Page
- Redesigned Menu Action context
+9 Commits, +685/-423 lines

 ### Detailed Updates, backend

1.9 (177.2025.07.23) - PF Rank Posts for Feed
- Added working personalized feed option
- Set default for feed to personal, will override (and added isUserSet)
- Added isUserSet for personalized feed options, so wont override
- Personalization options will default to 5/10 
- Fixed bug for adjusting email settings
- 231 pf rank posts for users

1.9 (178.2025.07.24) - Search Explore Page
- Added a new route to get newest 5 hashtags, users, and posts
- Fixed bug related to likes
- Getting likes for a post now provides more user information
- 251 search explore page  

v1.9 (179.2025.07.24) - v1.9 Release
- Personalized Feed is working and is set as default
- Stores posts that you’ve seen/indexes
- Personalization options defaults to 5/10
- Added new explore route with newest information
- Bug fixes
+15 Commits, +444/-83 lines

*autogen change notes

## What's Changed
* 1.9 (153.2025.07.24) - UI Improvements by @dkravec in https://github.com/social-novapro/social-frontend-plain/pull/154
* v1.9 (154.2025.07.24) - v1.9 Release by @dkravec in https://github.com/social-novapro/social-frontend-plain/pull/155


**Full Changelog**: https://github.com/social-novapro/social-frontend-plain/compare/v1.8.0...v1.9.0

```