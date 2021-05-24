## How To Get Started With Open Source Project Contribution

Open source is in your best interest, whether you're an individual, a corporation, a small business, a non-profit, or a government agency.
Contributing to Open Source can be a rewarding way to learn, teach, share and build experience. There are plenty of reasons why one/people would contribute to an Open Source Project, some of the reasons are: 

- To improve the software you rely on
- To find a mentor if need one
- Learn new skills
- Share your skills
- helps you gain a much deeper knowledge about the software
- helps your reputation and can leverage your career
- is fun and gives you personal satisfaction  

*What is your motivation to contribute to open source projects? Let me know by responding to this post or via Comment Section.*


### How can one Contribute to Open Source?  

Contributing does not necessarily mean to contribute to code, one can contribute to open source in many different ways, like:
- You can add a description to elaborate more or even give guidance to a given project.
- Add examples to show how the code works
- Write tutorials for the project
- Do a translation for a project
- You can answer questions about a project (Stack overflow, Reddit)
- Offer to mentor another contributor
- Fix typos and arrange the work folder correctly  

*All of the above ways count towards contributing to an open-source project.*  

### What To Note About Open Source Projects  

Every open source community is different. Each community has different people in it with different roles and rewards offered.

#### A typical open source project has these people: 

          
- **Author** - This is the person who created the project, have all the overall power can assign a new role to other members to help with projects maintain ace 
- **Owner** - The one has administrative ownership to the project (*can be the same person as the author*)
- **Maintainers** - Those who are responsible for driving the vision and goal of the project, is probably someone who feels responsible for the direction of the project and is committed to improving it
- **Contributors** - Those who are contributing in one way or another to the project, follow the same code review process, are subject to the same requirements on code style, and so on.
- **Community Members/Users** - These valuable members of the community can provide feedback about features, bug reports, and more.  

### A typical open source project should have these files too listed at the top:


- [License](https://choosealicense.com/) - If a project does not have an open-source license then it is not open-source. The license helps protects contributors and users. Businesses and savvy developers won’t touch a project without this protection. Wondering how to get one, click [Here](https://choosealicense.com/) to read more
- README - This is a manual that explains how to get started with the project. A good README should contain different things, Read more how to write a good README file [HERE](https://larymak.hashnode.dev/how-to-write-a-good-readme-file)
- Contributing - Helps people contribute and shows what type of contributors are needed(*this file is not a must*)
- [CODE_OF_CONDUCT](https://opensource.guide/code-of-conduct/) - A code of conduct is a document that establishes expectations for behavior for your project’s participants. Adopting, and enforcing, a code of conduct can help create a positive social atmosphere for your community.

To create an open-source project you will want to create an environment where people can share their challenges and do discussions, well that is made possible by the following tools:

- Issue Tracker - This is where people discuss issues related to the project
- Pull Request - This is where people review changes in progress
- Synchronous Chat Channel - This specifically meant for people to their ideas and do conversation (eg: Slack, IRC)

### How to find a Project to Contribute To :  

Now that you have figured out how an open-source project works, it's time to find a project to contribute to.  
Contributing works on all levels, don't overthink how you gonna do it, instead think of some of the projects you already use and how you can make a change or improve on them
> Research has shown that around 30% of casual contribution are documentation, typo fix or even translations  
If you are a first-timer, of which at some point everybody was, I have below given you some links that will get you started into the Open Source world:

- [Open Source Friday](https://opensourcefriday.com/)
- [Hebatica](https://habitica.com/static/front)
- [Pinax](https://pinaxproject.com/)
- [First Timers Only](https://www.firsttimersonly.com/)
- [Code Triage](https://www.codetriage.com/)
- [24 Pull Requests](https://24pullrequests.com/)
- [Contributor Ninja](https://contributor.ninja/)
- [First Contribution](https://github.com/firstcontributions/first-contributions)
%[https://github.com/firstcontributions/first-contributions]   
*In the world of open-source software, issues get reported and fixed pretty quickly. So, if you want to take on an issue, be sure to try to work on it promptly.*

### What to consider before you go open source  
Okay, so you can't wait to start your first OS project. Let's go through a few tips that might help you choose what to work on.
- #### Programming language  
The most fundamental technology behind any application is a programming language. Some most popular languages on GitHub are JavaScript, Python, Java, Ruby, and PHP. There is a multitude of projects that might suit your skills and taste. This does not mean the rest are not important they are too.
- #### Type of project  
After you've chosen the language you want to work in, you need to choose the type of project you prefer. Choose a topic that interests you.

### Criteria for Choosing A Good Project To Contribute To:

After you have found the one project you need, now make sure it meets the following criteria to be sure it is good for contribution:  
First, you will have to check:  
- Does it have a license file
- When was the latest commit done
- How many contributions does it have
- How often do people make commits

If all the above have done recently it means it has an active contribution, now we move into checking the second step:
- How many open issues are there
- How long does it take for maintainers to respond
- Is there an active discussion on an issue
- Are the issues getting closed
- How many pull requests are there
- How recently were the pull requests merged
- Do the pull requests get reviewed
- Do the maintainers thank people for contributing

If all the above conditions satisfy your needs to do a contribution then go for it and do it

### How To Submit a Pull Request  
If you are on this stage you definitely have found a project and you are good to go, the below steps will get you on the last step of submitting a pull request:  
First, What is a pull request? It is basically requesting for a git pull, getting someone to check your code before merging into another branch

- Fork the repository   -  
 at the top right hand, you will see the term fork, all you need to do is click it and you will have created the copy of the same project into your account, and the URL will change into
```
https://github.com/<YourUserName>/projectname
``` 
- Clone it to your local machine  
In your computer, if you have git installed open the CMD and run this command
```
git clone https://github.com/<YourUserName>/<projectname>
``` 
This will create a copy of the project into your local machine, Now that you have cloned the repo we will need to do two things:
- Create a Branch  
Change to the repository directory on your computer (if you are not already there): You can do that by
```
cd project folder name
``` 
now create a branch using the `git checkout command:  
```
git checkout -b your-new-branch-name
``` 
For example:  
```
git checkout -b lary-mak-blog
``` 
- Make necessary changes and commit those changes now you can make changes to the code. After doing some necessary changes and adding new files its time to add those changes to the branch you created, To see all changes made run the `git status` command:
```
git status
``` 
this show all recent changes made, now to add them use the `git add *` command 
```
git add *
``` 
now commit those changes using the `git commit` command: 
```
git commit -m "<initial commit> "
``` 
- Pushing Changes to GitHub  
This can easily be done using the `git push command:
```
git push origin <add-your-branch-name>
``` 
replacing `<add-your-branch-name>` with the name of the branch you created earlier.
- Submit Your Changes for Review
If you go to your repository on GitHub and refresh the page you'll see a Compare & pull request button. Click on that button.
Soon the maintainer will be merging all your changes into the master branch of this project. You will get a notification email once the changes have been merged.   

A pull request to another repo is similar to a “push”. However, it allows for a few things:
1. It allows you to contribute to another repo without needing administrative privileges to make changes to the repo.
1. It allows others to review your changes and suggest corrections, additions, edits, etc...
1. It allows repo administrators control over what gets added to their project repo.
 

- Where Next After Your First Pull Request?  
Congrats! You just completed the standard fork -> clone -> edit -> pull request workflow that you'll encounter often as a contributor! Now find a project and do more and be sure to watch out for the open-source month held by [Digital Ocean](https://www.digitalocean.com/) to participate in the [Hacktoberfest](https://hacktoberfest.digitalocean.com/)  and get a chance to win an amazing giveaway.

### Benefits of Contributing To Open Source:

- People that contribute to an open-source project get to know the technology at a much deeper level than they would be "simply" using the technology
- People can focus efforts on adding—and leveraging—features that will benefit businesses based on experience with what works and doesn't work in the real world.
- builds morale and reputation,
People who contribute to open source projects have access to other community members' insight and experience.
- Contributing to open source provides a clear view into the future of a project, 
- Resume builder - If you're on GitHub, a large portion of the things you do on that platform are public. Use this to your advantage by always doing your best when contributing and communicating with fellow contributors. You never know who is looking 

### Why You As A Developer Should Contribute To Open Source More
- Helps in writing cleaner code
- Increase community and peer recognition - Recognition can also end up with a lot of opportunities for potential employers.
- Helps in being prepared for the project
- Improve your coding skills

 
For more read the [Open Source Guide](https://github.com/github/opensource.guide/tree/8dad3dcca0bea99835202629ff227b0eb690d7e0) on GitHub

If You have read this far I really appreciate and would like to grow my community:  

Connect With me at [Twitter](https://twitter.com/larymak1) | [Insta](https://www.instagram.com/nextgencoders/) | [YouTube](https://www.youtube.com/channel/UCrT1ARRZfLOuf6nc_97eXEg) | [LinkedIn](https://www.linkedin.com/in/hillary-nyakundi-3a64b11ab/)  | [GitHub](https://github.com/larymak)

Do share your valuable opinion, I appreciate your honest feedback!  

Check out my other Blogs too:  
- [Build A Random Name Generator Using Python](https://larymak.hashnode.dev/build-a-random-name-generator-using-python)
- [How To Write A Good README File](https://larymak.hashnode.dev/how-to-write-a-good-readme-file)
- [Top Freelancing Tool For Developers](https://larymak.hashnode.dev/top-freelancing-tools-early-2021)
- [Top Apps To Learn Coding](https://larymak.hashnode.dev/top-apps-to-learn-coding)
- [Coding A Jokes App Using Python](https://larymak.hashnode.dev/coding-a-comicjokes-app-using-python)
- [The GMAIL Story](https://larymak.hashnode.dev/the-origin-of-gmail)
- [Useful Bash/Terminal Commands](https://larymak.hashnode.dev/some-useful-bashterminal-commands)  


See you in my next Blog article, Be Safe and Take care!!  
Enjoy Coding
