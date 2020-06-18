## Gitignore 
>`.gitignore` files help make sure you only get files you care in student repos without the potential of other file types sneaking in.  Most of the time this means you want the .java file and maybe some .txt or file types relevant to the project.  Usually, IDEs have several other file types that they need to work for that student's specific project but those files don't transfer nicely between IDEs or even different machines using the same IDE.  It is better to only receive the bare minimum you need and then open up the project in whatever environment you want so that you can get your own environment-specific files created.

To make changes or additions to any of the files here make a pull request on the repo, please.

This file is easiest to be in the root when getting started.  Though you can have other `.gitignore` files in subdirectories depending on what needs to get ignored unless you are comfortable with what you are doing a single `.gitignore` in the root will cover your needs if you include everything you want in there.

- The ignore file in the root covers multiple IDEs
    - This is the ignore file I use in the classroom
    - It is focused on Maven and Gradle projects therefore if not using those some setting may need changing
- This folder will have various `.gitignoreX` files
    - the X will be what that ignore file covers
    - in your own project, you will want to have the single file be `.gitignore` only no extra after it

These ignore files are not created by me.  Most have come from other GitHub repos but many come from the main [github gitignore repo](https://github.com/github/gitignore.git).  Another great service to getting an ignore file is [gitignore.io](https://www.toptal.com/developers/gitignore), I will probably switch the gitignore file I use before the start of the year by using this site to get me started.
