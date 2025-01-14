---
layout: page
title: Joel Foo's Project Portfolio Page
---

### Project: NUSCourseMates

NUSCourseMates is a desktop address book application used for keeping track of the courses your friends are taking. The user interacts with it using a CLI, and it has a GUI created with JavaFX. It is written in Java, and has about 10 kLoC.

Given below are my contributions to the project.

* **New Feature**: Incorporated the ability to modify the courses of a student in the address book into the `edit` function. 
  * What it does: Allows the user to change the courses of a particular student in the address book. 
    * With `edit 1 c/add-MA1521`, you can add MA1521 to student 1 in the address book. 
    * With `edit 1 c/del-MA1521`, assuming student 1 in the address book has MA1521 originally, you can remove MA1521 from student 1.
    * With `edit 1 c/MA1521-CS2030`, assuming student 1 in the address book has MA1521 originally, you can change student 1's MA1521 to CS2030. This is a convenience method that combines the power of both `add` and `delete` in one expression. 
  * Justification: This feature improves the product significantly because a friend in the address book can decide to take different courses at any point in time and the app should provide a convenient way for the user to update them.
  * Highlights: 
    * It is possible to chain any amount of each type of edit in a single command, providing unparalleled flexibility. 
      * For example, you can perform `edit 1 c/add-MA1521 c/del-CS2030 c/add-ST2334 c/CS2103T-MA2001`, and the changes will be performed in the listed order, from left to right. 
    * Implemented course validation, so that you can only add or delete a valid course.
    * Instead of having separate commands such as `addcourse` or `deletecourse`, maintaining the common interface `edit` provides much more flexibility and convenience. 

* **New Feature**: Added a `clear-courses` command that clears the courses of a specified student in the address book. 
  * What it does: Allows the user to remove all courses of a particular student in the address book.
  * Justification: This feature is extremely useful from a user perspective, as when a new semester begins, you would want to keep your friends, but want to remove all their courses. The alternative would be to manually remove courses for each student (by calling the `edit` function for each person in the address book), but that would be too cumbersome.

* **Code contributed**: [RepoSense link](https://nus-cs2103-ay2324s1.github.io/tp-dashboard/?search=joel-foo&sort=groupTitle&sortWithin=title&timeframe=commit&mergegroup=AY2324S1-CS2103-T16-1%2Ftp%5Bmaster%5D&groupSelect=groupByRepos&breakdown=true&checkedFileTypes=docs~functional-code~test-code&since=2023-09-22&tabOpen=true&tabType=authorship&zFR=false&tabAuthor=joel-foo&tabRepo=AY2324S1-CS2103T-T17-4%2Ftp%5Bmaster%5D&authorshipIsMergeGroup=false&authorshipFileTypes=docs~functional-code~test-code&authorshipIsBinaryFileTypeChecked=true&authorshipIsIgnoredFilesChecked=false)

* **Project management**:
  * Set up the project repo and codecov
  * Created the "developers" team for the Github organisation
  * Managed releases `v1.3` and `v1.3trial`

* **Documentation**:
  * User Guide:
    * Added documentation for the features `edit` and `clear-courses` ([\#125](https://github.com/AY2324S1-CS2103T-T17-4/tp/pull/125), [\#149](https://github.com/AY2324S1-CS2103T-T17-4/tp/pull/149))
  * Developer Guide:
    * Added implementation details of the `edit` feature ([\#125](https://github.com/AY2324S1-CS2103T-T17-4/tp/pull/125))

* **Community**:
  * PRs reviewed with constructive feedback provided ([\#52](https://github.com/AY2324S1-CS2103T-T17-4/tp/pull/52), [\#82](https://github.com/AY2324S1-CS2103T-T17-4/tp/pull/82), [\#94](https://github.com/AY2324S1-CS2103T-T17-4/tp/pull/94))
  * Contributed to forum discussions [\#86](https://github.com/nus-cs2103-AY2324S1/forum/issues/86)

* **Contributions beyond the project team:**
  * [Bugs reported during PE-D](https://github.com/joel-foo/ped/issues)
