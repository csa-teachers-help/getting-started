# Getting Started
> A README.md file can serve multiple purposes in a repository.  Usually, it is an explanation of what the project is, how to use the repo, do installs, etc. It is written in a markdown language which can be stylized to suit your needs.

There are multiple ways to use repos in the classroom.  When distributing assignments I usually create a "starter" repo on my personal GitHub account and then use the "starter code" option within GitHub Classroom to distribute the assignment with the "starter repo" files.

## Begin
1. Signup for a GitHub Account
2. Request an Education Account 
    - [GitHub Education Request Form](https://education.github.com/discount_requests/new)
3. While waiting for approval Create Organizations that can be your courses
    - Click on your profile icon on top right of GitHub 
    - Select "Your Organizations"
    - On page that loads click the "New Organization" button
    - Select the "Free" tier
4. Sign in to GitHub Classroom and create your Classrooms
    - [GitHub Classroom](https://classroom.github.com/)
5. If you are approved for Educational use
    - Make your Classroom organizations have access to private repos 
    - As of early 2020 this is done through the [Toolbox Page](https://education.github.com/toolbox/offers)
        - scroll to the bottom with the "GitHub" tile and click on the links there
        - a page will load with your organizations that you can apply a coupon to
6. If you are not approved for Educational use
    - You can still use GitHub classroom and everything here
    - You will have to work with public repos only for your classroom

**SPECIAL NOTE**
As of April 2020 GitHub gave unlimited private repos and collaborators on private repos to everybody with a GitHub account.  This means that when selecting the "Free" tier for an organization you may not need to apply an "extra" coupon to that organization because they used to give you the "Team" tier for discounted.  This "Team" tier was the lowest tier that offered unlimited private repos.  However, now that "Free" does the coupon may not be needed.  

Basically what I am long-windedly saying is the steps 5 and 6 may no longer be relevant to new organizations made.  I have not tested this idea as the organization I created and are using for the upcoming 2020/2021 school year were created and coupon applied 2 days before this news and feature was released.

### Ideas for how to use a repo for the classroom
- A way to distribute notes/lessons
    - If the repo is public or private (to the organization) students could fork the repo and add their own notes and understandings and then do a pull request back to the base repository
    - This will allow for a large collection of student notes where students are also contributing to the notes of the classroom

I have not done this idea personally.  I think it is a awesome idea but have not had the time to really sit down and plan out how it should flow or work in my classroom.  Anybody who is using GitHub for this purpose please provide some information to the [note-lesson repo](LINK_HERE).

- Distributing assignments (individual - private as part of an organization)
    - Create an assignment via GitHub Classroom and then share the invitation link with students
    - Students who accept the link with automatically clone the repository
        - If you provide starter "code" a README, etc. student repos will automatically populate with those files when cloned
    - A disadvantage to this is that once students accept the assignment their repo is completely separated from the starter "code" so if you update the start repo students will not see those changes
        - A workaround for this is to mass download (via the Classroom Desktop app or a shell script) all student repos for an assignment, go into all their repos make the changes and then push all those back to their individual repos
            - the shell script that I use for mass downloading and pushing is [here](https://github.com/jfiksel/github-classroom-for-teachers)
        - Once you have pushed back students can "pull" their own repo and get the updates
            - Pulling for students is a easy thing to forget if they are not used to doing it as part of the normal workflow habit
            - However, if a student does not pull and changes were made that can cause some issues and frustrating troubleshooting
            - There is no harm in pulling "no changes"
            - If students can get into the habit of making a pull request before trying to push or even before they start making changes a lot of frustration can be avoided


- Distributing assignments (individual - public as part of an organization)
    - Create a base repo and have student fork it
    - Students can then work on their own version and make pull requests back to the base when they are repo to have their work graded
    - An advantage to this is that any changes you need to make to the assignment can be done in the base then students can pull those changes into their own forked repos without you having to download and push back to them
    - A disadvantage to this is that students will be able to see each other repos and thereby code

Working with public repos does not need to be this "confusing" if you are not use to GitHub.  The thought behind suggesting the initial steps for public repos is to get students use to the typical open-source public repo GitHub process.

However, you can use GitHub Classroom to create an assignment and make all the repos public instead of private.  The process being described here is often how public project repos work on GitHub.  A disadvantage to having students have public repos is that they are all searchable through GitHub, Google, etc.  I would recommend caution of assignments being used with public repos especially if you are sharing assignments with another teacher or school.  Nothing is more disappointing when there is a great assignment but with a quick Google search you can find 30+ repos providing the answer.

Private repos do not eliminate cheating or sharing of code but is limits the public availability of the code.  The steps for making the code public are more work for the student.  Most people interested in cheated might not be interested in taking these extra steps to make the code public.
    