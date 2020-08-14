# Getting Started
> A README.md file can serve multiple purposes in a repository.  Usually, it is an explanation of what the project is, how to use the repo, do installs, etc. It is written in a markdown language that can be stylized to suit your needs.

**Special Note: If you see any changes that are needed in this file or want to add anything to this file or any file do so using a pull request.  This great video by Jake Vanderplas [simple pull request](https://www.youtube.com/watch?v=rgbCcBNZcdQ) does an excellent job of explaining how to do a pull request.  You do not need to use terminal/command line to clone the repo, create a new branch, or make the change.  All those steps can also be down through various Git GUI applications or even directly on GitHub itself, which means you would not need to "clone" down to your local machine.  Another excellent video showing off how to do this is from codebasics [pull request](https://www.youtube.com/watch?v=e3bjQX9jIBk)**

## Begin
The steps outline below are shown on in these two videos:
- [Getting Started with Classroom](https://youtu.be/ffhvoOY2sbg) 
- [Linking Everything Together Classroom](https://youtu.be/oCsdreoU2go)

GitHub also has an incredible YouTube channel with various helps and guides
- [GitHub Training Channel](https://www.youtube.com/c/GitHubGuides/videos)

1. Signup for a GitHub Account
2. Request an Education Account 
    - [GitHub Education Request Form](https://education.github.com/discount_requests/new)
3. While waiting for approval Create Organizations that can be your courses
    - Click on your profile icon on the top right of GitHub 
    - Select "Your Organizations"
    - On the page that loads click the "New Organization" button
    - Select the "Free" tier
4. Sign in to GitHub Classroom and create your Classrooms
    - [GitHub Classroom](https://classroom.github.com/)
5. If you are approved for Educational use
    - Make your Classroom organizations have access to private repos 
    - As of early 2020, this is done through the [Toolbox Page](https://education.github.com/toolbox/offers)
        - scroll to the bottom with the "GitHub" tile and click on the links there
        - a page will load with your organizations that you can apply a coupon to
6. If you are not approved for Educational use
    - You can still use GitHub classroom and everything here
    - You will have to work with public repos only for your classroom

**Note: As of April 2020, GitHub gave unlimited private repos and collaborators on private repos to everybody with a GitHub account.  This means that when selecting the "Free" tier for an organization you may not need to apply an "extra" coupon to that organization because they used to give you the "Team" tier for discounted.  This "Team" tier was the lowest tier that offered unlimited private repos.  However, now that "Free" does the coupon may not be needed.**

**Basically what I am long-windedly saying is the steps 5 and 6 may no longer be relevant to new organizations made.  I have not tested this idea as the organization I created and are using for the upcoming 2020/2021 school year were created and coupon applied 2 days before this news and feature was released.**

### Ideas for how to use a repo for the classroom
- A way to distribute notes/lessons
    - If the repo is public or private (to the organization) students could fork the repo and add their own notes and understandings and then do a pull request back to the base repository
    - This will allow for a large collection of student notes where students are also contributing to the notes of the classroom

I have not done this idea personally.  I think it is an awesome idea but have not had the time to really sit down and plan out how it should flow or work in my classroom.  Anybody who is using GitHub for this purpose please provide some information to the [note-lesson repo](https://github.com/csa-teachers-help/note-lesson).

- Distributing assignments (individual - private as part of an organization)
    - Create an assignment via GitHub Classroom and then share the invitation link with students
    - Students who accept the link with automatically clone the repository
        - If you provide starter "code" a README, etc. student repos will automatically populate with those files when cloned
    - A disadvantage to this is that once students accept the assignment their repo is completely separated from the starter "code" so if you update the start repo students will not see those changes
        - A workaround for this is to mass download (via the Classroom Desktop app or a shell script) all student repos for an assignment, go into all their repos make the changes and then push all those back to their individual repos
            - the shell script that I use for mass downloading and pushing is [here](https://github.com/jfiksel/github-classroom-for-teachers)
        - Once you have pushed back students can "pull" their own repo and get the updates
            - Pulling for students is an easy thing to forget if they are not used to doing it as part of the normal workflow habit
            - However, if a student does not pull and changes were made that can cause some issues and frustrating troubleshooting
            - There is no harm in pulling "no changes"
            - If students can get into the habit of making a pull request before trying to push or even before they start making changes a lot of frustration can be avoided

I have not used the GitHub Classroom Assistant, the desktop app since they updated it to include mass downloads.  I cannot speak to its ease or simplicity as I do the mass download and mass pushing through the shell script.  I do not know if the Assistant has mass pushing, I do not believe it does but could be mistaken.

This is the main function I use GitHub for in the classroom.  After one or two practice assignments using a tester account, which is described in the [creating repos repo](https://github.com/csa-teachers-help/create-org-repo), it is pretty easy to use GitHub as assignment distribution.  

- Distributing assignments (individual - public as part of an organization)
    - Create a base repo and have student fork it
    - Students can then work on their own version and make pull requests back to the base when they are repo to have their work graded
    - An advantage to this is that any changes you need to make to the assignment can be done in the base then students can pull those changes into their own forked repos without you having to download and push back to them
    - A disadvantage to this is that students will be able to see each other repos and thereby code

Working with public repos does not need to be this "confusing" if you are not used to GitHub.  The thought behind suggesting the initial steps for public repos is to get students to use to the typical open-source public repo GitHub process.

However, you can use GitHub Classroom to create an assignment and make all the repos public instead of private.  The process being described here is often how public project repos work on GitHub.  A disadvantage to having students have public repos is that they are all searchable through GitHub, Google, etc.  I would recommend caution of assignments being used with public repos especially if you are sharing assignments with another teacher or school.  Nothing is more disappointing when there is a great assignment but with a quick Google search, you can find 30+ repos providing the answer.

Private repos do not eliminate cheating or sharing of code but are limits the public availability of the code.  The steps for making the code public are more work for the student.  Most people interested in cheated might not be interested in taking these extra steps to make the code public.
