# Getting Started
> A README.md file can serve multiple purposes in a repository.  Usually, it is an explanation of what the project is, how to use the repo, do installs, etc. It is written in a markdown language which can be stylized to suit your needs.

There are multiple ways to use repos in the classroom.  When distributing assignments I usually create a "starter" repo on my personal GitHub account and then use the "starter code" option within GitHub Classroom to distribute the assignment with the "starter repo" files.

## Begin
1. Signup for a GitHub Account
2. Request an Education Account 
    - [GitHub Education Request Form](https://education.github.com/discount_requests/new)
3. While waiting for approval Create Organizations that can be your courses.
4. Sign in to GitHub Classroom and create your Classrooms
    - [GitHub Classroom](https://classroom.github.com/)
5. If you are approved for Educational use
    - Make your Classroom organizations have access to private repos via the [Benefits page](https://education.github.com/benefits) by clicking Upgrade next to the names at the bottom of the page
6. If you are not approved for Educational use
    - You can still use GitHub classroom and everything here you will have to work with public repos only for your classroom
7. Make your first repo on GitHub
    - Either in the organization or your own personal account
8. Create some practice assignments via GitHub Classroom
    - Provide starter code for some of them from the repos you made in step 

**Note** I usually have a "Tester" account that is added to all the organizations that was created with a separate email.  This account is invited to the organizations as a "member" just like students would be.  I use this account to see what students would see when accepting the GitHub Classroom assignments and what their repos would look like.  This account is also used for pushing back up to the student repo to see how I as the teacher would be able to access or download.  I really just use it for messing around with the two accounts via two different web browsers to see the interaction the teacher account (one with the education discount) can have with students (members who join the organization)

### Ideas for how to use a repo for the classroom
- A way to distribute notes/lessons
    - If the repo is public or private (to the organization) students could fork the repo and add their own notes and understandings and then do a pull request back to the base repository
    - This will allow for a large collection of student notes where students are also contributing to the notes of the classroom
- Distributing assignments (individual - private as part of an organization)
    - Create an assignment via GitHub Classroom and then share the invitation link with students
    - Students who accept the link with automatically clone the repository
        - If you provide starter "code" a README, etc. student repos will automatically populate with those files when cloned
    - A disadvantage to this is that once students accept the assignment their repo is completely separated from the starter "code" so if you update the start repo students will not see those changes
        - A workaround for this is to mass download (via the Classroom Desktop app or a shell script) all student repos for an assignment, go into all their repos make the changes and then push all those back via a shell script [here](https://github.com/jfiksel/github-classroom-for-teachers)
        - Once you have pushed back students can "pull" their own repo and get the updates
- Distributing assignments (individual - public as part of an organization)
    - Create a base repo and have student fork it
    - Students can then work on their own version and make pull requests back to the base when they are repo to have their work graded
    - An advantage to this is that any changes you need to make to the assignment can be done in the base then students can pull those changes into their own forked repos without you having to download and push back to them
    - A disadvantage to this is that students will be able to see each other repos and thereby code

### Ideas for README
- Use the README to explain the project details
- Outline specific objects you want students to focus on
- You can provide `inline` code hints to students
- Provide entire code block hints with syntax highlighting
```Java
public static void main (String[] args) {

}
```
- You can have students answer questions right inside the README
- You can provide comments back to them inside the README
    - If your comments are more code specific there are better options for that idea of which can be found in the feedback repo of the organization 

## Other files to include in student repos

### Gitignore
- `.gitignore` files are helpful is making sure you only get files you care in student repos without the potential of other file types sneaking in
- this file is easiest to be in the root when getting started
    - though you can have other `.gitignore` files in subdirectories depending on what needs to get ignored
    