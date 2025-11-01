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

When storing user profiles, both an array of objects and an object of objects can work, but they each have different advantages.

Arrays make it very easy to loop through every user using a for loop or methods like forEach and map. They are a good choice when you need to look at all users at once. The downside is that if you want to find a specific user, you usually need to search through the entire array until you find the correct object.

Objects make it faster and easier to find one specific user because you can access them directly by a key (like their username) without looping through everything. But objects are not as simple to iterate through compared to an array, especially if you want to perform an action on every user.

I would choose the object of objects approach for this situation because user lookup is very important in apps. Being able to find a user quickly by their username makes the app more efficient. The tradeoff is that looping through every user takes a little more work, but the speed of direct access makes up for it.