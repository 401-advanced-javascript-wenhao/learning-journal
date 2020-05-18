# Midterm Project Individual Submission - 5/17/2020

1. Describe your overall satisfaction level with your project results.  
Our miterm project was very successful. I like the ideas of our project and We completed almost every functionality that we planned to implement on this project. The presentation went very well, a lot of audience were interested in our project. The only thing did not go well is that the google OAuth didn't work on production environment. However, the overall outcome exceeds my expectation in the beginning of this project.

2. Briefly describe your group dynamic for the week.  
Team work was very important in this project. We used Trello to track our progress and we were on zoom call everyday to discuss, help each other, and work on project. When we stuck on some problems, we communicated well with each other so that others can help "unstuck" the problem. We had "merge party" everyday to show team members what features were going to add on staging branch so that everyone is on the same page about the project. Morgan worked really hard on this project. He did a lot of research about 'join collections' in the MongoDB.

3. Describe at least one difficulty you faced during project week and how you dealt with it. This difficulty could be technical in nature, or interpersonal.  
One of the difficulty I encountered during this project was merge conflict. I have done some group projects before, but I have not encountered any merge issues since everyone in the team was working on independent micro-service. In this project, we were working from same code base. So when someone did some refactor or change to base, it caused merge conflict. It scared me in the beginning but I realized that it is just a part of development process. I did some research about github merge conflict and also asked Morgan to walk me through how to solve merge conflict locally and in github. At the end of day, I learned a new skill - how to solve merge conflict and merge conflict doesn't scare me any more.

4. Describe at least one surprising success or failure you experienced during the week. 
On Day 4 of project week, I was helping one of my team member fix google OAuth. I took over his code and worked on top of that. I found out that his code was able to receive user information from google upon sucessful user signin without going through OAuth middleware. And we were not supposed to implement it in that way but I didn't have time to change it. Instead, I manipulated what I received from google and worked on top of that. In the end, google OAuth works properly locally and that was a small success but it didn't work on production environment which is a surprising failure. I am planning to do google OAuth from scratch myself next week. 

5. Describe changes you would make to your personal or team process that you can incorporate into your next team effort.  
I suggest we should set priorities about what features we should build first. In this project, we built the bearer authentication in the end and it made us rewirte most of the tests. If we set priorities in the planning phase, we can prevent this issue.

6. If there is anything else you wish us to know when assessing your contribution to the group project, please include it. Only members of the Instructional team will read these submissions, so you may be candid.  
In this project, I have contributed on base code, generic model, user model, basic authentication, sign-in route, sigh-up route, fixing google OAuth, bearer Auth, writing test, deployment etc.



