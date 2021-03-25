# Hello World Of GitHub Actions Using Docker

This was "Hello World" in Action Using Docker Container And Also How You can Create your Customized Action . Actions are individual tasks that you can combine to create jobs and customize your workflow. You can create your own actions, and use and customize actions shared by the GitHub community. 

### What is GitHub Actions?
[GitHub Actions](https://help.github.com/en/actions/getting-started-with-github-actions/about-github-actions) help you automate your software development workflows in the same place you store code and collaborate on pull requests and issues. You can write individual tasks, called actions, and combine them to create a custom workflow. 

### What is WorkFlow?
Workflows are custom automated processes that you can set up in your repository to build, test, package, release, or deploy any code project on GitHub.

### Steps To Create Your Own Action:
1. Add a ```Docker``` File.
2. Add an Encryption Script (```entrypoint.sh```).
3. Add an ```action.yml``` File.
4. Start Your Workflow File.
5. Run an Action From your Workflow File.
6. Trigger the Workflow.
7. Incorporte the Workflow.

> **Note**: [Click Here](https://lab.github.com/github/hello-github-actions!) for Official Course On [GitHub Labs](https://lab.github.com/)

## Code Of action.yml

```
name: "Hello Actions"
description: "This Was Hello World Of GitHub Actions Using Docker File for greeting"
author: "jaypatel15406@gmail.com"

inputs:
  MY_NAME:
    description: "Who to greet"
    required: true
    default: "World"

runs:
  using: "docker"
  image: "Dockerfile"

branding:
  icon: "mic"
  color: "purple"
```

```
## Output:
This is Hello World in GitHub Action Using Docker and My Name is Jay Patel and I am Student Developer and I am Pursuing CSE with Specialization Of Big data And Analytics.
```
### If You Encountering Error Such as Stated Below:-
![Error Image](https://github.com/jaypatel15406/Hello-World-GitHub-Action-Docker/blob/main/actions-error-image.PNG)

### Solution of above error:-

Try to use ```git reflog``` Command for Refresing Logs of Current GitHub Action file. Click [GitHub Reflog](https://git-scm.com/docs/git-reflog) for more information.   

# For More resources :

1.) [GitHub Actions Documentation](https://github.com/actions) <br/>
2.) [Features Of GitHub Action](https://github.com/features/actions) <br/>
3.) [GitHub Action Marketplace](https://github.com/marketplace?type=actions)
