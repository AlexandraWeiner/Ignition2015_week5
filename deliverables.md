#### Deliverables for week 5 Rails MVC
##### Odin Project Routing Guide Questions:
- What is the "Root" route?
   It is a route that tells the website where to take users when they click on your webpage. 
- What are the seven RESTful routes for a resource?
  The actions are index, show, new, create, edit, update, destroy.
- Which RESTful routes share the same URL but use different verbs?
  show, update, destroy and create, index.
- How do you specify an ID or other variable in a route?
  Prepend it with a colon.
- How can you easily write all seven RESTful routes in Rails?
  resources :posts
- What is the Rails helper method that creates the HTML for links?
  link_to "text", url

##### Odin Project Views Guide Questions:
- What is a layout?
  A preset piece of the webpage that rails creators formatted to every page to save time because it exists on all pages.
- What's the difference between a "view template" and a "layout"?
 View templates provide specific loops while layouts are general webpage formats.**
- What is a "Preprocessor"?
 A special way of executing ruby so specific features can loop etc and turn back into the original view. 
- Why are preprocessors useful?
  They allow you to have more complex functions for individual pages.**
- How do you make sure a preprocessor runs on your file?
 Name the file .erb. 
- What's the outputted filetype of a preprocessed *.html.erb file? What about a *.css.scss file?
HTML and CSS
- What is the difference between the <%= and <% tags?
The former displays what is returned in the tag. The latter is used when you don't actually want it displayed, but you still want the things inside to occur (like if each statements).
- What is a view partial?
A view partial allows for you to use HTML files across multiple files.
- How do you insert a partial into your view?
Name the file something like _user_form.html.erb and render them using <%= render "shared/some_partial"%>. **
- How can you tell that a view file is a partial?
The render syntax shows that the view file is a partial. 
- How do you pass a local variable to a partial?
 <%= render "shared/your_partial", :locals => { :user => @user } %>
- What's the magical Rails shortcut for rendering a User? A bunch of Users?
```
    <h1>Users</h1>
    <ul>
      <%= render @users %>
    </ul>
```
- What are asset tags and why are they used?
Asset tags locate files based on their name and render the HTML for them. They are used to grab images. 

##### Link to Odin Project Basic Routes, Views and Controllers repo: [my odin repo](<https://github.com/AlexandraWeiner/rest-tester/commit/0c687d7006aab2500179b1c3f49b528b095aad46>)
##### Link to Hartl's Rails Tutorial Chapter 5 repo: [my hartl's repo](<https://github.com/econno11y/Ignition2015_week4-sample_app>)
