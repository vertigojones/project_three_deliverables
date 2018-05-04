# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Geting started and scheduling your time

Most importantly, remember to **go slowly and be methodical**. That means you should be testing your changes in-browser as you write each line or so of code. Don't spend too much time trying to work out one particular problem - seek help! Time management is key. 
Always be commiting. Deploy early and often.

Here's a rough sketch of what you should do and in what order:

### Planning
* __MVP__. First design your _MVP_ (Minimum Viable Product). Have a plan for completing an MVP before getting too involved with _advanced_ features. Start writing your README file with some basic ideas. _Timebox_ any experimental or optional ideas, features, or technologies. Remember that good _time management_ is key!
* __User Stories__. Use _Trello_ to prioritize your User Stories / features. Focus on what is most important / critical to success.
* __Wire Frames__. Draft up a set of sketches to start from as you begin to design your app's front end. These sketches should be lightweight and rough so that you can easily iterate on them if you decide to add or remove features.
* __ERD__. Map out the data flow of your models by drawing your ERD. Keep your design strictly to a one-to-many relationship as your data flows from top to bottom. If you would like to tackle a many-to-many relationship, reach out to your instructor.

### Set Up Express
* __Create your back-end environment__. Start building out the Express environment for your first (main) model. Make sure to install all of your dependencies. The best reference for installing your app with Express can be found [here](https://github.com/ATL-WDI-Exercises/rails_bog_app/blob/master/Bog_MERN_Stack.md).
* __Initialize Git__. Create a new repisitory on _GitHub_ and link it to your new project. Remember to make it "public" and de-select the "Initialize this repository with a README" option. Then follow the steps.
* __Build your routes__. Using Express, build your RESTful back-end routes. Start with the main index route, then work on your individual CRUD routes (Create, Read, Update and Delete). **Test your routes in Postman**.
* __Commitment__. Commit your code early and often to _GitHub_ with good commit messages.
* __Branch__. Use _Git Branching_ for experimenting with different ideas and technologies.

### Set up React
*__Create your front-end environment__. Once you have CRUD working with your first model on the back-end (or at least have your main index routed correctly), then start building out your React environment. Again, make sure to install your dependencies. **All React dependencies should be install inside the "client" folder only**. The best reference for installing React can be found [here](https://github.com/ATL-WDI-Exercises/rails_bog_app/blob/master/Bog_MERN_Stack.md).

* **Begin with the end in mind.** Know where you want to go by planning with 
wireframes & user stories, so you don't waste time building things you don't need
* **Don’t hesitate to write throwaway code to solve short-term problems**
* **Read the docs for whatever technologies you use.** Most of the time, there is a 
tutorial that you can follow, but not always, and learning to read documentation is 
crucial to your success as a developer
* **Commit early, commit often.** Don’t be afraid to break something because you can 
always go back in time to a previous version.
* **User stories define what a specific type of user wants to accomplish with your 
application**. It's tempting to just make them _todo lists_ for what needs to get 
done, but if you keep them small & focused on what a user cares about from their 
perspective, it'll help you know what to build
* **Write pseudocode before you write actual code.** Thinking through the logic of 
something helps.

---

* __Basic styling__. Start to put together the HTML for the layout of your page, in accordance to your wireframes. Add some simple CSS if that helps you visualize how your page is going to look.