# SWI 2019 (/2020)

## SWI 2

These are materials for the [Software Engineering 2](http://is.mendelu.cz/katalog/syllabus.pl?kod=PEF:SWI2) course,
Tuesday group, 10 am local, taught on Mendel University in Brno, spring 2020, led by [@ZitaNemeckova](https://github.com/ZitaNemeckova) and [@himdel](https://github.com/himdel).

The topic is UI integration testing with cypress, the whole semester, except for (possibly) a UI intro workshop and a UX workshop.

If you need to contact us, please use the [ManageIQ/welcome](https://gitter.im/ManageIQ/welcome) channel on [Gitter](https://gitter.im). (You'll need a github login anyway.)  
Feel free to use that channel to share anything useful you've found :).

### Synopsis

If you have any suggestion about what to do next please leave a comment [here](https://github.com/RoadToSoftwareFactory/SWI-2019/issues/67)

| date | topic |
|-|-|
| 2020-02-18 | intro, organizational details |
| 2020-02-25 | setup, first steps |
| 2020-03-03 | How to login, click and find an element (Coronavirus version) |
| 2020-03-10 | Videoconference: Js tests in ManageIQ: Jasmine, Jest and Cypress (Coronavirus version) |
| 2020-03-17 | Inspector (Coravirus version)|
| 2020-03-24 | Writing your own UserScript (Coravirus version) |
| 2020-03-31 | ... |
| 2020-04-07 | ... |
| 2020-04-14 | ... |
| 2020-04-21 | ... |
| 2020-04-28 | ... |
| 2020-05-05 | ... |
| 2020-05-12 | ... |

### Local setup

You'll need:

* the VM with ManageIQ (https://himdel.eu/swi-miq.ova) (or to follow https://www.manageiq.org/docs/guides/developer_setup),
* node (10+)
* npm or yarn
* git
* Google Chrome (or Chromium)

Setup:

```
git clone https://github.com/ManageIQ/manageiq-ui-classic
cd manageiq-ui-classic
npm install
# edit cypress.json, change the URL to use the VM IP address instead of localhost - http://192.168.99.100:3000
npm run cypress:open
```

### How to log in, click and find an element (Coronavirus version)
As this is last minute this "contactless" class will be up to you, please have a look at about 1,5 hours of tutorials at https://docs.cypress.io/examples/examples/tutorials.html#Best-Practices . Feel free to send any testing questions our way. We can prepare some Q&A for next "contactless" class :) 

For backend people: https://docs.google.com/document/d/1ZktIxBIgc-HRLejDKcDJNOjXqd7fFluB95MjXnC4XT8/edit?ts=5e5d18b8#heading=h.b459vbu6h3g5


### Videoconference: Js tests in ManageIQ: Jasmine, Jest and Cypress (Coronavirus version)

At 10:00 please join us at https://bluejeans.com/8080963880 . We'll show you different js frameworks our project uses with examples (good and bad:)). Expected to take about one hour.

Recording: https://bluejeans.com/s/WtQ4W

To see code and not faces. Hover over the screen and adjust the view like below:
<img width="704" alt="Screenshot 2020-03-10 at 11 16 33" src="https://user-images.githubusercontent.com/9210860/76302910-16dcca00-62c1-11ea-8325-3e30d10e6111.png">

### Inspector (Coronavirus version)
Google Chrome: https://developers.google.com/web/tools/chrome-devtools (recommended)
Firefox: https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector

At 11:00 we''ll meet at https://bluejeans.com/8080963880 if you have any questions.

What you should learn from the tutorials:
- Elements tab
  - find an element and copy it(HTML) and its selector(jQuery)
  - add/remove CSS style to an element in Elements tab and in Console tab(using js/jQuery) 
  - delete/hide element
- Console tab  
  - read messages in Console tab
  - run an easy js code in js
  - clean messages, filter them by level/content
  - try out different `console` functions like `log, error, warn, dir, info, table` and anything else that looks good :)
- Network tab
  - reload a page and watch what happens in Network tab
  - select one request and look what's in Headers, Response tabs
  - simulate slow connection
  - disable cache - reloads js
  - block requests
- Application tab
 - look what you have in Cookies, Local Storage and Session Storage
 - try to edit/delete/add 
- Simulate Mobile Devices 
  - simulate Mobile version and play a bit with it :)  
- and anything else you find useful/interesting :)

### UserScript

Add your suggestion [here](https://github.com/RoadToSoftwareFactory/SWI-2019/issues/66)

At 10:00 we''ll meet at https://bluejeans.com/8080963880 as usual. It will be recorded so you can watch it later if the time isn't working for you.

Agenda:
- What is UserScript?
- What you need to start? Not much :)
- Let's try it works
- And write one that's actually useful :)

### Extra stuff 

Bunch of stuff that maybe interesting but is not required :) 

Tips for work in home situation from people with years of experience :) : 
https://www.youtube.com/watch?v=AOhJzmtjgxY&fbclid=IwAR2yLFSN5YsVaAjw_UsC9-h4E48Wxvm5E-Fpu1nEI6xT-LeC6iezm2Zexoo

### After coronavirus
Documentation https://docs.cypress.io/examples/examples/tutorials.html#Best-Practices
Tasks:
- Create a new test case
- Login - fill inputs and click `Log in`
- Commands - when you have a task that you have to do all the time
- `beforeEach`
- go to Configuration
- Edit and Save Server - try set different kinds of inputs and check if correct message is shown


---

## SWI 1

These are materials for the [Software Engineering 1](http://is.mendelu.cz/katalog/syllabus.pl?kod=PEF:SWI1) course,
Tuesday group, 11am local time, even-numbered weeks, taught on Mendel University in Brno, fall 2019, led by [@ZitaNemeckova](https://github.com/ZitaNemeckova) and [@himdel](https://github.com/himdel).

The topic will be Git, the whole semester.

If you need to contact us, please use the [ManageIQ/welcome](https://gitter.im/ManageIQ/welcome) channel on [Gitter](https://gitter.im). (You'll need a github login anyway.)  
Feel free to use that channel to share anything useful you've found :).


### Synopsis:

| date | topic |
|-|-|
| 2019-10-01 | Intro @ Red Hat |
| 2019-10-15 | (dekanske volno) |
| 2019-10-29 | Basics recap, Github, get it working |
| 2019-11-12 | Synchronization, Conflicts |
| 2019-11-26 | Rebase, graded exercise |
| 2019-12-10 | Advanced git |


#### 2019-10-15 (homework :))

Check out https://learngitbranching.js.org/ , go through the whole Introduction Sequence in the Main section, and look at the first Push & Pull exercise in the Remote section.
You can also try for yourself at http://git-school.github.io/visualizing-git/#free .


#### 2019-10-29 - Basics recap, Github, get it working

1. Recap of the git branching exercises

1. Make sure you have a github account, quick intro to github if needed

1. Get git working on your machines, make sure you can push to github

1. History, the why, what?  
  - `git log` - show what's what

5. Basics - `init`/`clone`, `git config`  
  - commits
  - branches
  - exercises, see below


#### 2019-11-12 - Synchronization, Conflicts

1. remotes

1. updating (pull vs fetch & merge...)

1. Conflicts  
  - branches (continued)
  - merge

1. `filter-tree`


#### 2019-11-26 - Rebase, graded exercise

1. rebase flow

1. `git rebase -i` - more real examples, get to try everything


#### 2019-12-10 - Advanced git

1. aliases, scripting, more configuration, .git directory structure


### Exercises

- Basics (2019-10-29)
  - Install some text editor if you don't like vim/nano
  - Set git username and email
  - Add a ssh key to your GitHub account
  - Fork [the SWI-2019 repository](https://github.com/RoadToSoftwareFactory/SWI-2019)
  - Clone the repository
  - Set up remotes
  - Create new branch
  - Create a file `<github login>/commit.md` inside the repository
  - Add some text to the file and create 1st commit
  - Add the hash of the 1st commit to the file and create 2nd commit
  - Add another line of text to the file, then add diff to the file and create 3rd commit
  - Create a pull request to the upstream repository


- Synchronization (3rd class)
Everybody open the file git-rebase.

Read the instructions carefully please :).

Every instruction should be one commit (this time).

  * so your first commit would just be deleting a line
  * and your second commit would change the other line
  * and so on :)

---

After you're done there..

1. Create a PR.

1. You should have a PR with 8 commits, **not** on your master branch - if not, try again :).

1. tell us - wait for a conflict

1. update your branch & resolve conflicts

1. reorder commits so that food-related commits are together

1. squash food-related commits into one

1. delete commit with your favorite color

1. rename commit with your favorite season to something in UPERCASE

1. edit commit with your favority city so it's Helsinki

---

## **EXAM**

Remember to read instructions from Git. It will tell you what to do :)

Update your master.

Everybody open the file `exam`. 

Read the instructions carefully please :). Use your notes or Google as much as you want. But do not talk with your classmates please.

Please switch to a new branch. 

Every line should be one commit (this time).

  * so your first commit would just be changing a line
  * and your second commit would change the other line
  * and rest is yes/no questions - one per commit


---

After you're done there..

1. Create a PR.

1. You should have a PR with 10 commits, **not** on your master branch - if not, try again :).

1. tell us - wait for a conflict

1. update your branch & resolve conflicts (hint: rebase) (20%)

1. reorder commits so that `next class`-related commits(questions 3, 5, 7) are together (10%)

1. squash `next class`-related commits into one (hint: you should use two `s` not three) (20%)

1. delete commit with question 1 (10%)

1. rename commits about your previous experience with Git (questions 2, 4) to be in UPERCASE (hint: you do not rename the commit at the same time as you write `r` but later) (20%)

1. edit commit that mentions SVN so answer is `Noooooooooooo` or `Yesssssssssss` (hint: you have to add changed file and amend commit) (20%)

1. push (with `-f`orce) and check it's ok (you should have 7 commits)

1. When done comment on your PR with something like `please review @himdel` or `please review @ZitaNemeckova`
  
---

The course will be followed by [Software Engineering 2](https://is.mendelu.cz/katalog/syllabus.pl?kod=PEF:SWI2).  
Details to be determined.
