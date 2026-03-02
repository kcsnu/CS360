1. Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
   
   Mere Metrics is a weight tracking app where users can log their daily weight, see all their past entries, set a goal weight, and get notified when they reach that goal. I made it to help solve the problem of not wanting to rely on memory or click through a bunch of screens just to check your weight entries. I think I made the flow pretty simple, where you log in or create an account, enter today’s weight, which then shows up under today's date. This setup works for a few different types of users, including the Routine Logger who wants a fast daily check-in, the Goal-Focused user who mainly wants to have a specific goal to track towards, and the Accountability user who wants an accurate record to look back on.

2. What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
   
   To make the app feel more user-centered, I tried to make the experience as smooth as possible for the user. For example, I combined the login and create account screen so users could easily see the two options to select. Also, the weight history screen shows a grid with both the date and weight so you can quickly see your progress without opening extra pages. From that same screen, users can add a new weight or update their goal. After each new entry, the app checks the saved goal and sends a notification to the user if it was reached. The SMS alerts are optional and permission based, so the app still works even if someone doesn’t want to enable texting.

3. How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?
   
   When I started coding, I referenced the Project Three rubric for the requirements. I also built the app in steps, where I first did the login system, then the SQLite database with Users, DailyWeights, and GoalWeight tables, and finally the SMS permission feature. My main approach was pretty consistent where I would take input from the screen, store or read it from the database, then refresh the grid so the screen always matches what’s saved. I think I would use this same method again in the future, since setting up the database early and building features in small pieces made things easier to test and felt less overwhelming.

4. How did you test to ensure your code was functional? Why is this process important, and what did it reveal?
   
   Testing was a big part of making sure everything worked. I used the emulator and walked through the full process over and over. I created accounts, logged in, added weights, updated and deleted entries, set goals, and checked that the grid refreshed correctly every time. For the SMS feature, I tested when permission was allowed and when it was denied. I wanted to make sure the app didn’t break if texting wasn’t available and that it only tried to send a message if permission was granted. I felt that this kind of testing mattered because it helped me catch issues with database updates and permission based behavior. 

5. Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?
   
   The biggest challenge for me was making sure the goal-reached texting feature didn’t mess up the rest of the app. Since it’s more of an extra feature, I had to design it so that if the user denies SMS permission, the app still runs normally. I also had to connect my earlier UI design to the real database without overcomplicating the code. I kept the history grid as the main center of the app and built everything around simple database actions, which helped keep the app working smoothly even when I added new features.

6. In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
   
   What I’m most proud of is how the data works from start to finish on the history screen. When someone adds a weight, it saves to the database, the grid then updates, and the app checks the goal weight to see if it should send an alert. It shows that I can build something that actually saves and uses data the right way and isn't just something that works one time.
   
   The app also connects what you see on the screen to the saved data and supports different user goals without adding a bunch of extra screens. I also tried to think ahead about launching the app. I made sure it works on newer Android versions and only asks for permissions that are really needed, which helped me focus on making the app reliable and that would help build user trust. 
