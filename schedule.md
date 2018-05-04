# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Geting started and scheduling your time

Most importantly, remember to **go slowly and be methodical**. That means you should be testing your changes in-browser as you write each line or so of code. Don't spend too much time trying to work out one particular problem - seek help! Time management is key. 
Always be commiting. Deploy early and often.

**Read the docs for whatever technologies you use.** Most of the time, there is a tutorial that you can follow, but not always, and learning to read documentation is crucial to your success as a developer!

**Write pseudocode before you write actual code.** Thinking through the logic of something helps.

**Consider your data flow and ERD**. It's easier to embed _both_ your second and third model into your first, rather than embed your third into your second. Think carefully about how you want to structure your models.

Here's a rough sketch of what you should do and in what order:

### Planning
* __MVP__. First design your _MVP_ (Minimum Viable Product). Have a plan for completing an MVP before getting too involved with _advanced_ features. Start writing your README file with some basic ideas. _Timebox_ any experimental or optional ideas, features, or technologies. Remember that good _time management_ is key!
* __User Stories__. Use _Trello_ to prioritize your User Stories / features. Focus on what is most important / critical to success.
* __Wire Frames__. Draft up a set of sketches to start from as you begin to design your app's front end. These sketches should be lightweight and rough so that you can easily iterate on them if you decide to add or remove features.
* __ERD__. Map out the data flow of your models by drawing your ERD. Keep your design strictly to a one-to-many relationship as your data flows from top to bottom. If you would like to tackle a many-to-many relationship, reach out to your instructor.

### Set Up Express
* __Create your back-end environment__. Start building out the _Express_ environment for your first (main) model. Make sure to install all of your dependencies. The best reference for installing your app with _Express_ can be found [here](https://github.com/ATL-WDI-Exercises/rails_bog_app/blob/master/Bog_MERN_Stack.md). **Reference your User Stories!**
* __Initialize Git__. Create a new repisitory on _GitHub_ and link it to your new project. Remember to make it "public" and de-select the "Initialize this repository with a README" option. Then follow the steps.
* __Initialize Heroku__. As soon as you have connected your project to _GitHub_, set up your _Heroku_ account also:

```bash
heroku create
heroku addons:create mongolab:sandbox
git push heroku master
```

* __Seed!__ Set up your database and seeds by hard-coding some sample data. It's best to create your data for all three models up front. Deploy to _Mongo_:

``node db/seeds.js``

Make sure that your seeds have been deployed by running _Mongo_:

```bash
mongo
show dbs
use folder_name
show collections
db.find.collection_name().pretty()
```

If your database is set up the way you want it to be, go ahead and seed to _Heroku_:

``heroku run node db/seeds.js``

* __Build your routes__. Using _Express_, build your _RESTful_ back-end routes. Start with the main index route, then work on your individual CRUD (Create, Read, Update and Delete) for your first model. **Test your routes in Postman**.
* __Commitment__. Commit your code early and often to _GitHub_ with good commit messages. Once you have commited each time to Git, commit also to _Heroku_.
* __Branch__. Use _Git Branching_ for experimenting with different ideas and technologies.

### Set up React
* __Create your front-end environment__. Once you have CRUD working with your first model on the back-end (or at least have your main index routed correctly), then start building out your _React_ environment. Again, make sure to install your dependencies. **All React dependencies should be install inside the "client" folder only**. The best reference for installing _React_ can be found [here](https://github.com/ATL-WDI-Exercises/rails_bog_app/blob/master/Bog_MERN_Stack.md).
* __Build your routes__. Using _React_, build your _RESTful_ front-end routes. Start with the main index route, then work on your individual CRUD (Create, Read, Update and Delete) routes for your first model. Put some time into planning your components and overall design flow.
* __Basic styling__. Work on some basic styling for your landing page. Consider using a style library, such as [Material-UI](https://www.material-ui.com/#/) or [Semantic-UI](https://react.semantic-ui.com/introduction). **Reference your Wireframes!**
* **Don’t hesitate to write throwaway code to solve short-term problems.**

### Work on your second model
* __Set up your back-end routes__. Try your best to get full CRUD on your second model in _Express_. Just like with your first model, work on the "show" route first. If you are short on time, jump into _React_ after getting your "show" route finished in _Express_. For reference, [this codealong](https://git.generalassemb.ly/atl-wdi/wdi-curriculum/blob/master/instructor_notes/react/react-fullstack-codealong.md) uses two models. **Reference your User Stories!**
* __Set up your front-end routes__. Work on your routes in _React_ to pull in your second model. Again, try and achieve full CRUD, but concentrate mainly on getting your "show" route to render in the front-end. Follow [the same codealong](https://git.generalassemb.ly/atl-wdi/wdi-curriculum/blob/master/instructor_notes/react/react-fullstack-codealong.md) for guidance.
* __Basic styling__. Work on some basic styling for your individual "show" page in _React_. Take note of your components and where they are being rendered on the page, as this helps with knowing _where_ to implement your styling. **Reference your Wireframes!**

### Work on your third model
* __Set up your back-end routes__. Try your best to get full CRUD on your third model in _Express_. Just like with your first and second models, work on the "show" route first. If you are short on time, jump into _React_ after getting your "show" route finished in _Express_. **Reference your User Stories!**
* __Set up your front-end routes__. Work on your routes in _React_ to pull in your third model. Again, try and achieve full CRUD, but concentrate mainly on getting your "show" route to render in the front-end.
* __Styling__. When you are in a place that you have everything rendering as it should on the front-end, start adding some pizzazz and make your project shine!

### Final Touches
* Finish README.
* Troubleshoot/Debug.
* If there is time, try and accomplish some of the stretch goals (listed on the README page).
* Deploy to [Heroku](https://www.heroku.com/).
