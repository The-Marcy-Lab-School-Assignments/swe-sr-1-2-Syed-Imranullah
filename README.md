# swe-sr-1-2

## Setup

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/how-tos/working-with-assignments#how-to-work-on-assignments).

Here are some useful commands to remember.

```sh
npm i                   # install dependencies
git checkout -b draft   # switch to the draft branch before starting

git add -A              # add a changed file to the staging area
git commit -m 'message' # create a commit with the changes
git push                # push the new commit to the remote repo
```

## Prompt

You are building an app and have to store data about user profiles. Each user profile is represented by an Object with an `id`, `username` and `password`. Below you will find two ways of grouping together these user objects, an array of objects and an object of objects:
```js
const usersArray = [
  {
    id: 214,
    username: 'Spongebob',
    password: 'dandelion'
  },
  {
    id: 592,
    username: 'Squidward',
    password: 'clarinet'
  },
  {
    id: 723,
    username: 'Patrick',
    password: 'whoareyoupeople???'
  }
]

const usersObject = [
  Spongebob: {
    id: 214,
    username: 'Spongebob',
    password: 'dandelion'
  },
  Squidward: {
    id: 592,
    username: 'Squidward',
    password: 'clarinet'
  },
  Patrick: {
    id: 723,
    username: 'Patrick',
    password: 'whoareyoupeople???'
  }
]
```

Compare and contrast these two options. Which would _you_ choose and why? What are the tradeoffs of each container? Consider how the container you choose makes it easy / difficult to find a user, to iterate through the users, etc...

### Response

Add your response here...
