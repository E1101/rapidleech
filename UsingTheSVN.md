This page contains information about using the SVN Repository

# Structure #

The structure used in this repository is similar to the structure recommended by Subversion:
  * **tags/** Directory in which the code of each released version is freezed.
  * **trunk/** Branch where the development of Rapidleech v2 is focused only recommended for advanced users.
  * **branches/** Directory in which all branches of Rapidleech are stored.


# Committing #

There are a series of good habits that must be accomplished to ensure a correct functioning of the repository:

Before commiting a change, you should update your code to the last revision and check it works flawlessly. You must think the possible consequences of your changes. In case of doubt, you must consult in the forum. You cannot commit a change in a part maintained by other people before consulting them before. The commits must always be related to the purpose of the changes. You cannot commit different changes with different purposes.

Remember that **every** commit must have a comment, indicating what modify/add and the propose of this change.

Finally, we have a few tags to indicate what is the reason of the commit, that tags are used to create the changelog, so don't use it if you think that your change should not appear in that changelog:

  * `[`FIX`]` or `[`FIX #000000`]`: This tag is to mark that the commit is to fix a bug that are there since the previous version. If the bug are reported in the bugtrack (mantis) the bug id must be attached).
  * `[`FEATURE`]`: When we finish the implementation of the new feature, we need to indicate it with this tag (only in the final commit when the feature is considered stable and complete).
  * `[`CHANGE`]`: If we change a current feature, for example modifying the behaviour.
  * `[`SECURITY`]`: If the commit fix a security bug, it need to be tagged with a special tag.

# Fixing a bug #
When a bug is fixed, you must indicate in the comment of the commit an identifying number, accompanied by a precise explanation of the problem and solution. For example:
```
BUG: #189203
Rapidleech Don't have a platform for help the developers feedback.
Now, we use google code as developers platform. 
```