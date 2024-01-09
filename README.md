# cse477website
# CSE-477 Website Michigan State University Web Development
This was my CSE 477 Michigan State University MSU website for Professor Mohammad Ghassemi built using HTML, CSS, Javascript and Python Flask. Contains interactive piano, user signup and login, different user chatroom. 


# [Web Application Development] Homework 1

## Purpose

The purpose of this assignment is to provide with hands-on experience with frontend development including:

1. How to write and structure HTML documents.
2. Best practices for styling reactive HTML documents using CSS.
3. Building interactive client-side applications using HTML, CSS, and Javascript.

## Assignment Goals

Your high-level goal in this assignment is to develop a mobile-friendly professional webpage with:

1. **A Home page**: providing information about you, and your professional background. 
2. **A Projects page**:  providing descriptions and links to functional web projects you are working on.
3. **A Piano project:** providing a fully functional piano web application built in HTML CSS and Javascript (with a hidden twist.)  

Your implementation should satisfy both the General Requirements, and Specific Requirements detailed in the sections below;  to help you grasp the overarching goal and requirements more concretely. Please note; your implementation does not have to look identical to the example solution. As long as you achieve the Specific and General requirement below, your assignment is complete.

## Specific Requirements

For each of the three assignment goals listed above, we provide a section that outlines the specific requirements associated with that goal, below: 



##### Home page requirements

We've provided a placeholder home page for your application called [`home.html`](flask_app/templates/home.html); You will need to add a [`<header>`]([](https://www.w3schools.com/tags/tag_header.asp))  [`<nav>`](https://www.w3schools.com/tags/tag_nav.asp)  [`<main>`](https://www.w3schools.com/tags/tag_main.asp) and  [`<footer>`](https://www.w3schools.com/tags/tag_footer.asp) section to this template. Each HTML sections should satisfy the *Structure*, *Content*, *Style*, and *Interactivity* requirements outlined in the table below. Any `CSS` and `Javascript` should be imported separately, not included in your HTML file. 

|                          | [`<header>`]([](https://www.w3schools.com/tags/tag_header.asp)) | [`<nav>`](https://www.w3schools.com/tags/tag_nav.asp)        | [`<main>`](https://www.w3schools.com/tags/tag_main.asp)      | [`<footer>`](https://www.w3schools.com/tags/tag_footer.asp)  |
| ------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Structure**            | -  always appears at the top of the page                     | - appears beneath the `<header>`                             | - appears beneath the`<nav>`                                 | - always at the bottom of the page.                          |
| **Content**              | - a banner image (e.g. [this one](flask_app/static/main/images/banner.jpg)) | - Name of the assignment<br /><br />- Link to the `home.html` page <br /><br />- Link to the `projects.html` page <br /><br />- Link to your resume.<br />- Link to your LinkedIn page (embedded in [an icon](flask_app/static/main/images/social-linkedin.png)) <br /> | - your name<br /><br />- photo of you<br /><br />- brief description of you<br /><br />- fun fact about you | - the copyright symbol © , followed by your name             |
| **Style**                | - banner images should cover the entire header area; i.e. no [margin](https://www.w3schools.com/css/css_margin.asp) and no [padding](https://www.w3schools.com/css/css_padding.asp)<br />- banner size should scale with screen [viewing height](https://www.w3schools.com/cssref/css_units.asp) and [viewing width](https://www.w3schools.com/cssref/css_units.asp) | - name of the assignment should be on the left of the nav bar<br /><br /> - All links should appear on the right of the nav<br /><br />- The [opacity](https://www.w3schools.com/css/css_image_transparency.asp) of the links should change on [hover](https://www.w3schools.com/cssref/sel_hover.asp).<br /><br />- navbar size should scale with screen [viewing height](https://www.w3schools.com/cssref/css_units.asp) and [viewing width](https://www.w3schools.com/cssref/css_units.asp) | - all text should be centered and [justified](https://www.w3schools.com/cssref/css3_pr_text-justify.asp)<br /><br />- the name, photo and breif description should appear  in a row of content with two equal sized columns. The row should have a maximum [viewing height](https://www.w3schools.com/cssref/css_units.asp) of 50vh, and [viewing width](https://www.w3schools.com/cssref/css_units.asp) of 80vw.<br /><br />- the photo should cover the entire area of the left column; the name and description should appear on the right column; [text overflow](https://www.w3schools.com/cssref/css3_pr_overflow-y.asp) should be handled with the scroll bar.<br /><br />- the fun fact should appear in seperate line of content.<br /> | - should have a color that is distinct from the color of `<main>`.<br /><br />- all text should be centered and justified. |
| **Mobile Interactivity** | - None required                                              | - the nav links should disappear when the screen size is less than `650px`, and be replaced with a [menu bar](flask_app/static/main/images/menu-bar.png) that, when clicked, displays the links.<br /><br />- the LinkedIn Icon should be replaced with text that says "LinkedIn" | - any two column content should transition into single column content when the screen size less than `650px`; [text overflow](https://www.w3schools.com/cssref/css3_pr_overflow-y.asp) should be `visible`; all single column content should have a viewing width of 80vh. | - None required                                              |



##### Projects page requirements

We've provided a placeholder projects page for your application called [`projects.html`](flask_app/templates/projects.html);  it will use the same *Structure*, *Style*, and *Interactivity* conventions as the Home page. The only section that will differ between the Projects page and the Home page is the *Content* in `<main>`. The *Content* requirements include:

* A single column row of content explaining the purpose of the page (i.e. to show off your project work).

* A two-column row of content that shows an [image of a piano](flask_app/static/main/images/piano.jpeg) on the left; and a description of the piano project on the right, with a link to `piano.html`
* clicking the image of the piano should take you to the `piano.html` page.



**Piano project requirements**

We've provided a placeholder page for your piano application called [`piano.html`](flask_app/templates/piano.html);  it should use the same *Structure*, *Style*, and *Interactivity* conventions as the Home page. Within  `<main>`, you will place:

* <u>In HTML:</u> At the top of the page should be the following poem: ""*Behold piano great and old, it's master slumbers in far off cold, If you wish to see anew, call out to it - we see you.*""
* <u>In HTML and CSS:</u> Under the poem will be your piano. It should have 10 white keys, 7 black keys, and the name "The Great Old One". The piano can be constructed by [layering HTML elements](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Positioning/Understanding_z_index/Adding_z-index). For instance, you can make each key in the piano a separate `<div>` with an appropriate size, ID, etc. It should look something like this at the end:

![piano-1](documentation/piano-1.png)

* <u>In Javascript:</u>  Create [a mouseover event listener](https://developer.mozilla.org/en-US/docs/Web/API/Element/mouseover_event) to detect when the mouse hovers over any key of the piano, and temporarily reveal the keyboard keys that control the piano; it should look something like this when your mouse is hovered over any of the keys:

![piano-2](documentation/piano-2.png)

* <u>In Javascript:</u> Create a [keydown event listener](https://developer.mozilla.org/en-US/docs/Web/API/Document/keydown_event) to detect when a given key is pressed (e.g. the S key), and alter the style of the corresponding HTML element that represents that key to indicate it was pressed. If the S key were pressed, for instance, you should temporarily see something like the image below. I suggest looking into the [transform](https://developer.mozilla.org/en-US/docs/Web/CSS/transform) and [box-shadow](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow) in CSS if you want to replicate the effect in my example, but you can choose to style it another way too; for instance, by temporarily changing the key's [background color](https://www.w3schools.com/cssref/pr_background-color.asp), or changing the key's size. 

![piano-2](documentation/piano-3.png)

* <u>In Javascript:</u> Use the [keyCode](https://keycode.info/) from keypress events captured by the keydown event listener to identify which key was pressed. Next, use the following [JSON object](https://www.w3schools.com/whatis/whatis_json.asp) to map the keyCode to a url containing the sound of the note you need to play. You can play these notes by passing the corresponding url to an [Audio() constructor](https://developer.mozilla.org/en-US/docs/Web/API/HTMLAudioElement/Audio) in Javascript:

```json
const sound = {65:"http://carolinegabriel.com/demo/js-keyboard/sounds/040.wav",
                87:"http://carolinegabriel.com/demo/js-keyboard/sounds/041.wav",
                83:"http://carolinegabriel.com/demo/js-keyboard/sounds/042.wav",
                69:"http://carolinegabriel.com/demo/js-keyboard/sounds/043.wav",
                68:"http://carolinegabriel.com/demo/js-keyboard/sounds/044.wav",
                70:"http://carolinegabriel.com/demo/js-keyboard/sounds/045.wav",
                84:"http://carolinegabriel.com/demo/js-keyboard/sounds/046.wav",
                71:"http://carolinegabriel.com/demo/js-keyboard/sounds/047.wav",
                89:"http://carolinegabriel.com/demo/js-keyboard/sounds/048.wav",
                72:"http://carolinegabriel.com/demo/js-keyboard/sounds/049.wav",
                85:"http://carolinegabriel.com/demo/js-keyboard/sounds/050.wav",
                74:"http://carolinegabriel.com/demo/js-keyboard/sounds/051.wav",
                75:"http://carolinegabriel.com/demo/js-keyboard/sounds/052.wav",
                79:"http://carolinegabriel.com/demo/js-keyboard/sounds/053.wav",
                76:"http://carolinegabriel.com/demo/js-keyboard/sounds/054.wav",
                80:"http://carolinegabriel.com/demo/js-keyboard/sounds/055.wav",
                186:"http://carolinegabriel.com/demo/js-keyboard/sounds/056.wav"};
```

* <u>In Javascript:</u> When the sequence of keys "weseeyou" is typed on your piano it should awaken the great old one! More specifically, (1) your piano should gradually fade away and be replaced by the [image of the great old one](flask_app/static/piano/images/texture.jpeg), (2) you should play the following [creepy audio](https://orangefreesounds.com/wp-content/uploads/2020/09/Creepy-piano-sound-effect.mp3?_=1) and (3) the piano should no longer respond to key presses; at the end, the piano should look something like this:

![piano-4](documentation/piano-4.png)


# [Web Application Development] : Homework 2

## Purpose

The purpose of this assignment is to provide you with hands-on experience with backend development including:

1. [Python Flask](https://flask.palletsprojects.com/en/2.0.x/) - a backend for your web application.
2. [MySQL](https://www.mysql.com/) - a relational database to store and retrieve data for your application.
3.  [Jinja](https://jinja.palletsprojects.com/en/3.0.x/) - a tools for generating dynamic HTML content.

## Assignment Goals

Your high-level goal in this assignment is to extend your professional webpage from Homework 1 to include:

1. **A Database**:  allowing you to store persistent information used by your web application.
1. **A Resume page**: providing a HTML version of your Resume (rather than a .pdf). 
2. **A Feedback form**:  Allowing visitors to provide feedback anywhere on your web application.

Your implementation should satisfy both the General Requirements, and Specific Requirements detailed in the sections below. Please note; your implementation does not have to look identical to the example solution. As long as you achieve the Specific and General requirement below, your assignment is complete.

#### 1. Database requirements

For this portion of the assignment, you will specify a database that allows you to store information used by your web application. This will involve three tasks:  

1. **Specify several database tables** by adding `.sql` files to `database/create_tables` folder; more specifically you will create:

   * **`experiences.sql`**: contains the `CREATE TABLE` statement for the `experiences` table, which describes all the experiences you had at each position in the `positions` table ; the table should contain the following columns:

     * `experience_id`: the primary key, and unique identifier for each experience
     * `position_id`: a foreign key that references  `positions.position_id` 
     * `name`: the name of the experience.
     * `description`: a description of the experience.
     * `hyperlink`: a link where people can learn more about the experience.
     * `start_date`: the state date of the experience.
     * `end_date`: the end date of the experience.

   * **`skills.sql`**: contains the `CREATE TABLE` statement for the `skills` table, which describes all skills associated with each of the experiences in the `experiences` table ; the table should contain the following columns:

     * `skill_id`:  the primary key, and unique identifier for each skill
     * `experience_id`: a foreign key that references  `experiences.experience_id` 
     * `name`: the name of the skill
     * `skill_level`: the level of the skill; 1 being worst, 10 being best.

   * **`feedback.sql`**: contains the `CREATE TABLE` statement for the `feedback` table, which contains user feedback about your website; the table should contain the following columns:

     * `comment_id`: the primary key, and unique identifier for each comment.

     * `name`: the commentators name

     * `email`:  the commentators email

     * `comment`:  The text of the comment

       

2. **Specify the initial data that will populate your tables** by adding `.csv` files to `database/initial_data`; more specifically, you will create (or update):

   1. **`institutions.csv`**: contains data that will be ported into the `institutions` table on initialization of the app.

   2. **`positions.csv`**: contains data that will be ported into the `positions` table on initialization of the app.

   3. **`experiences.csv`**: contains data that will be ported into the `experiences` table on initialization of the app.

   4. **`skills.csv`**:  contains data that will be ported into the `skills` table on initialization of the app.

      

3. **Extend the [database utility](flask_app/utils/database/database.py)** by adding functions that create tables, insert data, and fetch resume data; more specifically, you will populate the following empty function in the database utility:

   1. **`createTables()`**: should create all tables in your database by executing each of the  `.sql` files in `database/create_tables`, and populating them with the initial data provided in `database/initial_data`. Note that `createTables()` is called in `__init__.py` and will therefore be executed upon creation of your application.

   2. **`insertRows()`**: should insert rows into a given table; more specifically, the function should take the table name, a list of column names, and a list of parameter lists (i.e. a list of lists) and execute the appropriate `INSERT` query.

   3. **`getResumeData()`**: should return a nested `dict` that hierarchically represents the complete data  contained in the `institutions`, `positions`, `experiences`, and `skills` tables. Tables should be nested according to their foreign key dependencies. Here's an example of what the the returned data should look like:

      ```json
      {1: {'address': 'NULL',
              'city': 'East Lansing',      
             'state': 'Michigan',
              'type': 'Academia',
               'zip': 'NULL',
        'department': 'Computer Science',
              'name': 'Michigan State University',
         'positions': {1: {'end_date'        : None,
                           'responsibilities': 'Teach classes; mostly NLP and Web design.',
                           'start_date'      : datetime.date(2020, 1, 1),
                           'title'           : 'Instructor',
                           'experiences': {1: {'description' : 'Taught an introductory course ... ',
                                                  'end_date' : None,
                                                 'hyperlink' : 'https://gitlab.msu.edu',
                                                      'name' : 'CSE 477',
                                                    'skills' : {},
                                                'start_date' : None
                                              },
                                           2: {'description' : 'introduction to NLP ...',
                                                  'end_date' : None,
                                                  'hyperlink': 'NULL',
                                                  'name'     : 'CSE 847',
                                                  'skills': {1: {'name'        : 'Javascript',
                                                                 'skill_level' : 7},
                                                             2: {'name'        : 'Python',
                                                                 'skill_level' : 10},
                                                             3: {'name'        : 'HTML',
                                                                 'skill_level' : 9},
                                                             4: {'name'        : 'CSS',
                                                                 'skill_level' : 5}},
                                                  'start_date': None
                                              }
                                          }
                          }
                      }
          }
      }
      ```

      

#### 2. Resume page requirements

For this portion of the assignment, you will write code that generates a dynamic HTML version of your Resume. This will involve two tasks:  

1. **Complete the `resume.html` template** by adding html and jinja statements that dynamically transform the data returned by `getResumeData()` into a dynamic, and <u>mobile friendly</u> resume page; more specifically, your resume page should:
   * <u>For each institution</u>, display:
     * `name` of the institution; this should be left justified.
     * location information for the institution (`department`,`address`, `city` etc.); this should be right justified. 
     * <u>For each affiliated position,</u> display:
       * `title`; this should be left justified
       * `start_date` and `end_date`; this should be right justified.
       * `responsibilities` of the position.
       * <u>For each affiliated experience,</u> display: 
         * `name` of the experience; this should be a hyperlink if the `hyperlink` field is not NULL.
         * `description` of the experience
         * <u>For each affiliated skill, display</u>:
           * `name` of the skill. 
2. **Be mindful of your styling**; while I have not specified specific constraints on the styling here, the content should:
* Look good on both mobile and desktop screens.
  
* Only display a field if it is not `"NULL"` or `None`
  
* Denote the hierarchical relationships in the source data using font-sizes, colors, bullets, etc.



#### 3. Feedback form requirements

For this portion of the assignment, you will generate a feedback form that allows users to send feedback on your site from anywhere in your web application; this will involve three  tasks:

1. **Add an html feedback form** to the `layout.html` template (along with any supporting CSS and JavaScript). The form should contain:

   *  `action` attribute that sends the data to the `/processfeedback` route in `routes.py`.
   *  `method`, and `enctype` attributes that specify a [POST request](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/POST).
   * The form should contain four `<input>` elements:
     * `name`: a text field that captures the name.
     * `email`: a text field that captures the email.
     * `comment`:  a text field that captures the comment.
     * `submit`: a button that submits the form.
   * The form should be styled such that:
     * the `position` of the form centers it in the screen, even as a user scrolls up or down.
     * the `display` of the form makes it initially invisible.

2. **Add a button that toggles the visibility of the feedback form** to the `layout.html` template. More specifically;

   * When the button is pressed the form should become visible.

   * The button to toggle the feedback form should show up on every page of your application and should always be visible.

3. **Process and store the feedback:**

   * In `routes.py`,  add a route and function to handle the feedback data submitted by the users. Within the route, access the submitted data via `request.form`. It should look something like this:

     ```python
     @app.route('/processfeedback', methods = ['POST'])
     def processfeedback():
     	feedback = request.form
     ```

   * within the `/processfeedback` route, add code that:

     * Inserts the form data into the `feedback` table within the database.

     * Extract all feedback from the `feedback` table
     * Render a template `processfeedback.html` that transform the feedback data into a dynamic, and <u>mobile friendly</u> feedback page; 

     

#### 4. OPTIONAL: Create a Favicon for your website

Visit [this website](https://favicon.io/logo-generator/) to quickly generate a favicon for your site. Add this line to your HTML head; note that the value of the `href` attribute should be the location of the favicon, which may differ from what I'm showing below.

```HTML
<link rel="shortcut icon" href="static/main/images/favicon.ico">
```

# [Web Application Development]: Homework 3



## Purpose

The purpose of this assignment is to provide hands-on experience with basic security, authentication and asyncryonous communication technologies for your web application, including:

1. Session management,
2. Password encryption and user authentication and,
3. Asynchronous communication technologies.



## Assignment Goals

Your high-level goal in this assignment is to extend your webpage from Homework 2 to include:

1. **An Authentication System**:  allowing user authentication, and restricted access to certain components of your application.
2. **A Chat System**: allowing you and a guest user of your web application to engage in a live text-based conversation. 
3. **An Editable Resume [Only Required for Honors Option]**:  allowing the site owner to add and edit parts of the resume from Homework 2, using the website.

Your implementation should satisfy both the General Requirements, and Specific Requirements detailed in the sections below;  to help you grasp the overarching goal and requirements more concretely, [see the Homework overview video](https://youtu.be/NZzUMxTJKr4). Please note; your implementation does not have to look identical to the example solution. As long as you achieve the Specific and General requirement below, your assignment is complete.

#### 1. Authentication System Requirements 

For this portion of the assignment, you will generate the authentication system for your web application; this will involve two main tasks:  

1. **Extend the database utility to support sensitive data storage and authentication** by extending/completing the following code:

   * **`createUser(email, password, role)`**: Should create database entries for your users given an email, password and role (`guest`, or `owner`). The function should only add a user to the database if they do not already exists (i.e. if there is no matching email). The password of the user should be encrypted using [Scrypt](https://docs.python.org/3/library/hashlib.html) before being stored; you may use the `onewayEncrypt` function provided in the utility. The function should also return information about the success or failure of user creation.

   * **`authenticate(email, password)`**: Should check if a given email and encrypted password combination exist in the database. The function should  return information about the success or failure of the authentication.

2. **Enabling login and logout functionality for your application** by extending/completing the following code:

   * **`@app.route('/login')`**:  Should render the `login.html` template. The HTML template should contain two inputs that capture the email and password of the user, as well as a button that submits the credentials for authentication to `@app.route('/processlogin')`  using an asynchronous POST request via [AJAX](https://flask.palletsprojects.com/en/2.0.x/patterns/jquery/). If `@app.route('/processlogin')` indicates that the authentication was a failure this should be noted on the page; more specifically, your page must dynamically show how many times the authentication attempt has failed. If the authentication is a success, the user should be redirected to `/home`.

   * **`@app.route('/processlogin')`**:  Should be configured to process a POST request containing credentials for authentication. More sepcifically, the tool should extract the credentials from the request, and check if the user's email and password match a value in a the database using the `authenticate` method from the database utility. If the authentication is successful, the user's session should be updated to contain an encrypted version of their email; see below for an example:

   ```python
   session['email'] = db.reversibleEncrypt('encrypt', form_fields['email']) 
   ```

   The status of the authentication should be be returned as a JSON object to the AJAX handler in `login.html` for further action; see below for an example:

   ```
   return json.dumps(status)
   ```

   * **`@app.route('/logout')`**:  Should remove the `email` field from the session using [session.pop](https://pythonbasics.org/flask-sessions/) and redirect the user back to `/home`.

   * **`templates\shared\layout.html`**: The navigation bar should be updated to include a login/logout option. More specifically, when a user is logged in, they should see the option to logout; conversely, when a user is logged out, they should see the option to login.



#### 2. Chat System Requirements 

For this portion of the assignment, you will write code creates a live chat system in your web application. This will involve two tasks:  

1. **Complete the chat.html template** by adding HTML, CSS and JavaScript that allows users to see ongoing messages, enter their own messages, and leave the chat. The template already contains a functional implemention of `socket.io` for streaming messages in real time from the Client's interactions with `chat.html` to the `def joined(message)` in `routes.py`.  More specific requirements follow:

   * <u>Room Entry</u>: all users in the chat should see a message indicating when a given user "has entered the room"; this component was already completed for you. 
   * <u>Message Entry:</u> all users in the chat should see the messages entered by all other users.
   * <u>Room Derture:</u> all users in the chat should see the messages indicating when a user has "left the room". There should be a button on the page that allows the user to leave the chat.
   * <u>Message Styling:</u> all messages related to the site owner should be in blue and right justified; all other messages should be grey and left-justified.

2. **Add SocketIO processors in routes.py:** by writing any additonal  `@socketio.on(...)` decorated functions to `emit` data back to `chat.html`

   

#### 3. An Editable Resume

**PLEASE NOTE:** This section is only required if you want to complete the course as an Honors Option. Given the optional nature of this component, the instructions are not be as detailed:

1. Update your `/resume` page page so that when the owner of the site is logged in, they can add/edit all resume content; this should be something like the profile editors on social media platforms, but the specific implementation is up to you. You will receive credit for this insofar as the owner can: 
   * add new entries to your resume
   * edit existing entries
   * you were mindful of styling. 
