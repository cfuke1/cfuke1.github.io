---
layout: essay
type: essay
title: "Software Engineering Reflection"
# All dates must be YYYY-MM-DD format!
date: 2024-05-09
published: true
labels:
  - Software Engineering
  - Coding Standards
  - Agile Project Management
---

### Introduction

Software Engineering in the modern day requires many skills and a strong coding background. However, I believe that beyond those things, there are primary two skills that are responsible for creating a strong foundation for software engineers. These are proper Coding Standards and effective Agile Project Management. With these two skills in one’s belt, they can be effective and efficient in any project that they take part of. In this essay, I would like to break down these two skills, and explain how I developed them during my time taking ICS 314. 

### Coding Standards

In my opinion, Coding Standards are one of the most important things to have in mind when typing code. Coding standards are a fundamental practice that benefit software development by enhancing consistency, readability, and security. Code consistency is ensuring that code is written in predictable and understandable patterns. Keeping code consistent is especially helpful for when different types of objects are needed, as consistent code can be replicated and changed easily. Throughout my time in ICS 314, my code was primarily kept consistent by ESLint. ESLint is a code analysis tool for JavaScript that scans code and points out errors and inconsistencies. These are a few examples of ESLint’s feedback. 
```
ESLint: 'Student' is defined but never used. (no-unused-vars)
ESLint: Trailing spaces not allowed. (no-trailing-spaces)
ESLint: Unused import Student from '../components/Student';
```
It is very helpful for keeping code consistent, as it checks for duplicate fragments of code, and also creates its own spacing for the code that is used. 
However, I would say that ESLint primarily helped with my code’s readability. Whatever variables, imports, or functions weren’t used in my project, ESLint would make note of, and recommend me to delete. If not for this, I am sure that many lines of code would have ended up in my project without a purpose. These could cause problems, but they mainly make the code more difficult to read. Without good readability, comprehending what certain lines of code actually do becomes very difficult very fast. This becomes compounded in group settings, where multiple people need to work on multiple files at once. 
Security is the last, and arguably one of the most important coding standards to keep in mind during software engineering. Ensuring that data is kept safe is your responsibility as a software developer. Breaches of information are serious problems in the realm of software engineering, and you are responsible for keeping the information of everyone who uses the software you develop safe. Security at its most basic level is ensuring that bad actors cannot exploit the users of your software or exploit the software itself for malicious purposes. In this regard, ESLint was not able to help me anymore, and ensuring that my code was safe and secure was all my responsibility. I made sure that my code was secure by making use of the MongoDB database and the publication subscriptions that it allowed me to implement. MongoDB is a database program that allows for large storage of data. It comes with subscriptions that can only allow users with certain roles to access certain data collections. This made it so that it would be impossible for anyone to access data that they weren’t allowed to access, as it would never be on the web application in the first place if there was no subscription. 

Without proper coding standards in place, developers may end up writing code that is difficult to understand and becomes difficult to fix. This can be difficult to manage with multiple developers working on the same project, as the different styles of coding can interfere with each other and hinder progress. This is why over the course of ICS 314, I eventually found ESLint to be very useful. It took time for me to get used to using ESLint in my code, but I believe that it was crucial for me to keep my code clean and functional. Also, I think that during the Final Project, everyone having ESLint was a huge help in allowing us to work on one file at the same time. Beyond web application development, coding standards are something that would be useful in all types of projects. Whether it’s coding for security, banking, or video games, having clean and consistent code that follows proper coding standards will always be beneficial to productivity. In the future, if I work with JavaScript again, I could see myself making use of ESLint again, because of all the benefits it brings to my code. Even if I were to not work in JavaScript again, I feel that ICS 314 has equipped me with the mental tools I would need to keep my coding standards in mind no matter what software engineering endeavor I take on. 

### Agile Project Management 

I would consider Agile Project Management to be one of the hardest parts of software engineering. Very frequently, software engineers work in teams to solve problems and create applications. In my opinion, coding may be one of the hardest things to do with other people, due to the somewhat confusing way that contributions are made to projects. These come in the form of pushes, pulls, and merges, the latter of which can frequently lead to bugs and setbacks in code. I believe three key points are responsible for supporting the whole of effective agile project management. 

The first of these points is an incremental approach towards writing and pushing code. This effectively means writing small features and functionality in the main code, as opposed to adding multiple things at once. This ensures that bug-fixing is easier, with less code to skim over, which allows code to be fixed faster if there are merge conflicts. Also, less code being pushed into the main branch means that there is less likely to be errors, and if there is, there would be much less than if a larger block of code were pushed. In group settings, an incremental approach becomes even more important, due to the fact that setbacks on the main branch will set the entire group’s progress back as a whole. Also, designating members to work on specific, small features would ensure that no member ends up working on something that is already being worked on. This saves crucial development time, and helps to make sure that deadlines are consistently being met. 

The second of these points is Effective Collaboration and Communication. This may seem very obvious, but I feel that it can get overlooked if a team is not organized. If not accounted for, members of a group can become confused as to what needs to be worked on and what has been fixed. Throughout the ICS 314 final project, my group used a GitHub project board to keep track of our progress and which members were working on certain things. 

 <img class="img-fluid" src="../img/eslint.png">

This ensured that everyone was able to make progress on their own time, and not have to ask to make sure what was finished and what was not. It also allowed us to double up on things that were difficult to program, so individual members wouldn’t need to take them on by themselves. It was important for us to constantly be pushing our finished commits to the branches, and then to main. This is so no member would ever end up with work that was behind in commits, and their effort wouldn’t go to waste. I would recommend project boards for any type of group work in software engineering, because they expedite the organization of people very effectively. However, effective collaboration and communication goes far beyond just a project board. Over the course of the final project, my group also used Discord to communicate with each other, and inform each other of what we were doing. Communication is key when working with other people, and always letting your group members know what branches have been modified is important. If multiple branches get merged into main and break it, fixing those bugs would become a nightmare with so much modified code. Proper communication and collaboration also is good for ensuring that all members can contribute to the project in meaningful ways. Finding out where individual members’ skills lie in the context of your project allows the group to work as fast as possible together by best utilizing each member. 

The last pillar of agile project management is a clear vision of where the project is going and what its final boundaries and functionalities are. Very often, projects can become bloated with features and functionality, which can end up with failed promises and disappointment with the final product. A clear vision of how the final product should function should be created at the beginning of the project’s development, and if time allows, more functionality should be added after the base product has been completed. This ensures that what was originally planned for the product will be delivered on. One way of creating a clear vision for a final product are mockup pages. This is an example of one that my group and I used for our ICS 314 final project. 

 <img class="img-fluid" src="../img/eslint.png">

Images like these were made for every single page that our web app would need. This was important, and gave us a template to work off of, as opposed to completely working in the dark while coding our project. While working, I would constantly refer back to the mockup pages we created to make sure that I was sticking to the original project’s vision. Although having a clear vision for the product at the beginning of a project is important, I still think that improving upon that vision during the project is fine, as long as it is done responsibly. Consumer and business demands can change with time, and if new features need to be added, it is okay for the team to change their final vision. This just needs to be done responsibly and incrementally, as to not bloat the product with unnecessary features, and allow the team to keep up with the increased work. Most importantly, the team should deliver on what has originally been promised first, and then focus on adding extra functionality later. 

### Conclusion

Overall, these two skills primarily bolster proper cooperation. Using ESLint to document code not only helps the original editor, but also helps everyone else on the team understand their code. Cooperating with consumers by writing safe and secure code ensures that data breaches won’t cause problems in the future. Incremental approaches and proper communication all reinforce the design team’s cooperation, allowing the project to be done faster. Being able to work with others is of paramount importance in a software engineering setting, whether it be with a team, with consumers, or with business executives, proper cooperation will make the result of a successful project much more likely. I would recommend all software engineers, new or old, to try and develop these skills on their next endeavor, as I think they could go a long way in improving the efficiency and enjoyment of software engineering as a whole. 






