## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
A cookie is sent with the HTML request with information about the user of the site.
* What’s the difference between a session and a cookie?
A session is a specific type of cookie that keeps track of a user as they use the site.
* What’s a flash and when do you want to use flashes?
A flash is a short message that can be sent to the user to confirm an action, or display an error.
* Why do people say “HTTP is stateless”?
HTTP does not remember who you are. As Nick E. said, it is like Dory from Finding Nemo.
* What’s authentication? Explain.
Authentication checks that the user of the site is who they say they are (with a passoword).
* What’s the difference between authentication and authorization?
Authentication makes sure the person is who they say they are, authorization is what priveledges and abilities they have.
* What’s a before filter?
A before filter is a bit of code that runs before any of the methods in a class.
* How do we keep track of a user once they’ve logged in?
A new session is created and destroyed when they logout.
* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
namespace: when you want the url to reflect the behavior of the routes. For example: admin. Then you can make sure no default users can get to any */admin/* pages. Nesting resources is for when a model belongs to another model. I think the best example is how jobs belong to a company.
* At a high level, what tools can you use to implement authorization? How would you use them?
We used bcrypt to hash passwords so none were sent as plaintext.

* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
An enum is a way to store a column in a table as a number that corresponds to the position of an array.

* What are some strategies you can use to keep your views DRY?
1. partials
2. general css classes
