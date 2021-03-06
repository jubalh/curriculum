---
layout: page
title: DonorsChoose Retrospective
---

In July 2012, the first Hungry Academy class divided into six teams of four to create projects supporting the mission of [DonorsChoose.org](http://donorschoose.org).



### Requirements

As this was the final project of Hungry Academy, the requirements were kept very light, allowing maximum freedom to the teams.

The main expectation was that the final product reflect the nearly three weeks the team put into it.

### Inputs

Teams had the opportunity to build upon two data sources:

1. The public DonorsChoose.org API which offered information about current projects
2. A dataset which held extensive records about past projects, donors, donations, gift cards, etc

### Process

#### Teams

* Group 1: Christopher Maddox & Mark Tabler & Chris Anderson & Travis Valentine
* Group 2: Austen Ito & Jonan Scheffler & Jacqueline Chenault & Charles Strahan
* Group 3: Andrew Glass & Mary Cutrali & Mike Silvis & Andrew Thal
* Group 4: Michael Chlipala & Jan Koszewski & Elise Worthy & Melanie Gilman
* Group 5: Conan Rimmer & Edward Weng & Nisarg Shah & Tom Kiefhaber
* Group 6: Michael Verdi & Darrell Rivera & Horace Williams & Daniel Kaufman

#### Planning

To begin the process, teams spent two hours generating three ideas each. The ideas were then presented to the rest of the class, and the class voted on which one the team should pursue.

#### Development Cycle

Teams met with Matt and Jeff twice per week to review progress, help them hone the scope of their work, and give feedback on the user experience. Technical advising, at this stage of the course, was very light as teams were expected to know how to do things on their own.

### Evaluation

#### Internal / Code

The first phase of evaluation was a peer code review. Participants were paired up with someone from another team and together reviewed a third team's code. The process went like this:

* Clone the project code from Github
* Review 

### Results

The teams all presented their projects to an audience of engineers and a representative from DonorsChoose.

### Reference URLs

* Group 1:
  * Code: https://github.com/chrismanderson/DonorWidget
  * Production: http://donors-widget.herokuapp.com/
* Group 2:
  * Code: https://github.com/seedthelearning/
  * Production: http://www.seedthelearning.com
* Group 3:
  * Code: https://github.com/andrewglass1/teacher-center
  * Production: http://teachercenter.herokuapp.com
* Group 4: Elise Worthy, Jan Koszewski, Melanie Gilman, Mike Chlipala
  * Code: https://github.com/mikesea/donors_select
  * Production: www.donorsselect.com
* Group 5:
  * Code: https://github.com/nisargshah100/charity-chain
  * Production: http://charitystreak.herokuapp.com
* Group 6:
  * Code: https://github.com/worace/donors-choose-wireframe
  * Production: http://donorschallenge.herokuapp.com/

### Peer Reviews

This morning you'll pair up to critique aspects of each other's projects and make suggestions for improvement. Each pair will be assigned a project and an area of focus.

#### Protocol

Get together with your pair and:

##### 1. Setup for Development (<15 minutes)

1. Clone the code from Github
2. Get it running by following the README
3. Install any dependencies
4. Generate seed data if needed
5. Make sure that all the tests pass
6. Get it running through the browser in development

##### 2. Evaluate (~30 minutes)

1. Evaluate your area of focus
2. Make notes about weaknesses
3. Create a github issue for **each** discrete issue you find
4. Include evidence from the code (*ex: "The challenge model is inadequately tested"*)

##### 3. Patch (~45 minutes)

1. Create a new git branch
2. Implement one your suggestions from the evaluation
3. Verify that it works
4. Push to github
5. Submit a pull request which includes notes about *why* you made these changes
6. Return to the master branch
7. `GOTO` step 1

### Round 1 -- 9:00 to 10:30

#### Reviewing Models

* Project 1: Travis Valentine, Melanie Gilman
* Project 2: Jan Koszewski, Edward Weng
* Project 3: Michael Verdi, Elise Worthy
* Project 4: Tom Kiefhaber, Austen Ito
* Project 5: Horace Williams, Christopher Maddox
* Project 6: Michael Chlipala, Mike Silvis

##### Questions to Consider

* Do the models use good encapsulation?
* Is there a separation of public/private methods?
* Are the methods well named?
* Are the methods small, comprising a single purpose?
* Can some of the Ruby style be simplified?
* Is there documentation for the public methods?
* Is potentially-reusable code pulled out into modules?
* Has "magic data" been pulled out to constants? Or a configuration file/initializer?

#### Reviewing Tests

* Project 1: Darrell Rivera, Jacqueline Chenault
* Project 2: Andrew Glass, Chris Anderson
* Project 3: Charles Strahan, Jonan Scheffler
* Project 4: Conan Rimmer, Daniel Kaufman
* Project 5: Mary Cutrali, Andrew Thal
* Project 6: Mark Tabler, Nisarg Shah

##### Questions to Consider

* Are there unit tests for each model?
* Are there integration tests for each major screen/view?
* Are there controller tests for any API calls?
* Do the tests adequately cover the application's functionality?
* Do they use good style and take advantage of test framework features? (`let`, `before`, etc)
* Do they stub/mock out any external services?
* Do the unit tests truely only test one component?

### Round 2 -- 10:30 to 12:00

#### Revewing UX/UI and Views

* Project 1: Nisarg Shah, Michael Verdi
* Project 2: Mary Cutrali, Melanie Gilman
* Project 3: Chris Anderson, Conan Rimmer
* Project 4: Horace Williams, Austen Ito
* Project 5: Darrell Rivera, Daniel Kaufman
* Project 6: Andrew Glass, Mike Silvis

##### Questions to Consider

* Are the views well organized? (naming, formatting)
* Do they make effective use of partials to promote reuse and avoid repetition?
* Do they use view helpers or model methods to avoid logic in the views?
* What parts of the visual design work well? What needs improvement?
* How is the error feedback? What happens when you put in invalid data?
* Is the site responsive? Would you want to keep using it?

#### Reviewing Controllers

* Project 1: Michael Chlipala, Jacqueline Chenault
* Project 2: Travis Valentine, Edward Weng
* Project 3: Christopher Maddox, Jonan Scheffler
* Project 4: Andrew Thal, Charles Strahan
* Project 5: Mark Tabler, Elise Worthy
* Project 6: Tom Kiefhaber, Jan Koszewski

##### Questions to Consider

* Are the controller methods very short?
* Do they create a minimum number of instance variables, or should they use a facade object?
* Is the logic pushed down to the model?
* Are dependencies (like the caching mechanism) adequately pushed down to the model layer?
* Are queries done in a secure way to avoid SQL injection, privledge escalation, etc?
* Is there any documentation for API methods about the inputs and outputs?

### Merging Patches

Now recollect in your project group and review the patches submitted to your code. 

* If they're good, merge them in and post a thanks comment.
* If they're not, write a detailed note about why the patch was rejected.
* Make sure everything still works correctly and get it up in production for tomorrow!