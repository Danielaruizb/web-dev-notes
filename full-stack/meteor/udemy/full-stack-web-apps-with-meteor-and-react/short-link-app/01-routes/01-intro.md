# Short Link App
* [live web app URL](http://short-lnk.herokuapp.com/)
* [short-lnk github](https://github.com/andrewjmead/short-lnk-meteor-course)

## Client-Side Routing Options
User Accounts, Authentication, and Routing

We are using **client-side** routing as opposed to **server-side** routing

**server-side** routing requires the server to send back markup for every page, this means your browser has to go through a full page refresh

In **client-side** routing, the **client-side** JavaScript watches the **URL** for changes and when it changes, it simply swaps out the content (In our React app we may render one Component instead of another Component)

**note** Meteor will server up the exact same content regardless of the **URL**. It is our job on the client to take note of that **URL** and do something about that (_and we would show some content depending on some **URL**_)

This is a very common pattern and is not unique to **Meteor** or **React**. Other frameworks like Angular have **client-side** routing (_It really is the way forward now for all new apps_)

### Walk through example of client side routing
* [live web app URL](http://short-lnk.herokuapp.com/)

### Meteor.com recommends FlowRouter
[**URL**s and Routing](https://guide.meteor.com/routing.html)

## We won't use **FlowRouter**
Why?

Check out [its' Github](https://github.com/kadirahq/flow-router)

* Not updated in a year
* Lots of issues piling up and not being addressed

### Iron Router
Also lots of issues and not many commits

[iron router github](https://github.com/iron-meteor/iron-router)

## Due Diligence
Before you use a Library due some due diligence

* Make sure the Library is still updated
* Make sure the community is actively committing
* Make sure the issues aren't piling up without a bunch of unanswered questions

### React Router
[github for react router](https://github.com/ReactTraining/react-router)
* Has lots of stars
* Lots of recent commits
* Not many unanswered issues
* React Router is worked on by a great community of developers who care

![Big Picture Map](https://i.imgur.com/HMYflBH.png)

* Meteor
    - Add manipulate a collection
    - Log in/Log out
* Routes (_will all get mapped to a set of React Components_)
    - `/` (_root route - shows log in page_)
    - `/signup` (_for new accounts_)
    - `/links` (_main private page, where you manage your links_)
    - `/blablabla` (_404 handler_)
    - `/_blasomebla` (_special **URL** that starts with an underscore and will enable us to do some redirecting_)