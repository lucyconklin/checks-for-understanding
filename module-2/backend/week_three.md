## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?
```rails new app_name ```
2. What do Models generally inherit from in rails?
```class ModelName < ActiveRecord::Base```...
3. What do Controllers generally inherit from in a rails project?
```ApplicationController```
4. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
```resources :horses, only: [:show]```
5. What rake task is useful when looking at routes, and what information does it give you?
```rake routes``` I typed this about 1000 times over the weekend
6. What is an example of a route helper? When would you use them?
```horse_path(@horse)``` it is a built in shortcut for links to a route/view
7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?

pass

8. What are strong params and why are the necessary?
strong params limit the params that come through a form. Good for making the application more secure.
9. What role does `form_for` play in helping us create our forms?
```form_for```wraps everything in a <form> tag, and handles labels/links/translation to params.
10. How does `form_for` know where to submit the user's input?
path helper?
11. Create a form using a `form_for` helper to create a new `Horse`.
<%= form_for @horse do |f| %>
<%= f.label :name %>
<%= f.input :name %>

<%= f.label :favorite_snack %>
<%= f.input :favorite_snack %>

<%= f.submit 'Submit Horse' %>
12. Why do we want to validate our models?
To make sure the objects have all of the information they need before being saved.
