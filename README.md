# Getting Started
> A README.md file can serve multiple purposes in a repository.  Usually, it is an explanation of what the project is, how to use the repo, do installs, etc. It is written in a markdown language which can be stylized to suit your needs.

There are multiple ways to use repos in a classroom.  When distributing assignments I usually create a "starter" repo on my personal GitHub account and then use the "starter code" option within GitHub Classroom to distribute the assignment with the "starter repo" files.

### Ideas for how to use a repo for the classroom
- A way to distribute notes/lessons
    - If the repo is public or private (to the organization) students could fork the repo and add their own notes and understandings and then do a pull request back to the base repository
    - This will allow for a large collection of student notes where students are also contributing to the notes of the classroom
- Distributing assignments (individual - private as part of an organization)
    - Create an assignment via GitHub Classroom and then share the invitation link with students
    - Students who accept the link with automatically clone the repository
        - If you provide starter "code" a README, etc. student repos will automatically populate with those files when cloned
    - A disadvantage to this is that once students accept the assignment their repo is completely separated from the starter "code" so if you update the start repo students will not see those changes
        - A workaround for this is to mass download (via the Classroom Desktop app or a shell script) all student repos for an assignment, go into all their repos make the changes and then push all those back via a shell script [here] ( https://github.com/jfiksel/github-classroom-for-teachers )
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
    