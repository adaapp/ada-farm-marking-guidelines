# Ada Farm Assignment: Marking Guide

Thanks for helping out on the marking for the Advanced Programming Assignment. This guide ensures a consistency across all markers, outlining a standardised approach we must all follow.

## 1. Familiarise yourself with the coursework

Please start by [reading the assignment](SD4AdvancedProgrammingAssignment.docx) 

## 2. View the marksheet samples

N.B. The quality criteria have changed since Cohort 3 completed the coursework.

* [Pass](marksheet-samples/pass.pdf)
* [Higher Pass](marksheet-samples/pass-higher.pdf)
* [Merit](marksheet-samples/merit.pdf)
* [Distinction](marksheet-samples/distinction.pdf)
* [Highest Distinction](marksheet-samples/distinction-highest.pdf)

## 3. Familiarise yourself with the criteria and quality breakdowns

These are all encoded in Airtable. There are four quality options for each section, with a description that will be given to a student in their marksheet. When assigning a mark to a section, work out which broad quality category their work fits into. Give zero marks if they've not attempted the section.

Airtable will take the ceiling (i.e. rounded up to the nearest integer) of your mark, divide it by the number of marks available for that section, and multiply it by four to arrive at the quality level.

### Section 1: Essay and UML (if you are just marking Ada Farm, please ignore this section)

1. Programming Approaches (5 marks)

* Quality 1: Incorrect reference to imperative or declarative programming paradigms. Code indicated as declarative is actually imperative, or vice versa.
* Quality 2: Definitions of an acceptable quality. Code correctly indicates different approaches but is formatted badly.
* Quality 3: Good definitions of imperative and declarative approaches with a good comparative analysis and good code examples.
* Quality 4: Excellent definitions of imperative and declarative approaches with excellent comparative analysis and code examples.

2. Programming Paradigms (15 marks)

* Quality 1: Incorrect or muddled definitions. Missing examples of systems suited to each paradigm.
* Quality 2: Acceptable definitions but examples are inappropriate.
* Quality 3: Good definitions and good examples.
* Quality 4: Excellent definitions and examples.

3. UML (10 marks)

* Quality 1: UML notation not used and only basic information given. Some relationships are unnecessary or incorrect.
* Quality 2: OK use of UML notation with largely correct relationships. 
* Quality 3: Good use of UML notation clearly showing correct relationships and properties. 
* Quality 4: Excellent use of UML notation clearly showing relationships, properties and methods.


### Section 2: Ada Farm: General quality

1. Code quality (10 marks)

* Quality 1: Very poor quality suggests a very low programming ability.
* Quality 2: Style suggests a lack of confidence with programming, or a lack of effort on this assignment.
* Quality 3: A good, confident approach is evidence of a good command of programming.
* Quality 4: Excellent approach in a confident style. 

2. Refactor (5 marks)

* Quality 1: No attempt to change the code that's there – new code is in exactly the same format.
* Quality 2: Only a basic attempt to add new features or try new approaches.
* Quality 3: Lots of new code shows confidence with the code base.  
* Quality 4: An entirely new approach executed to a high standard.

3. Time sheet / git commits (5 marks)

* Quality 1: No time sheet submitted and incomprehensible git commits.
* Quality 2: Timesheet fails to grant any insight into the process.
* Quality 3: A good timesheet combined with a good commit history provides great insight into the process.
* Quality 4: An excellent and detailed timesheet and a clear, descriptive commit history.

### Section 3: Ada Farm: Criteria

1. Farm pass criteria (20 marks)

* Quality 1: Only one of the standard requirements (animals, crops, and the market) implemented, and no further technical concepts found. 
* Quality 2:  Only one of the standard requirements (animals, crops, and the market) implemented, and one or more technical concepts found.
* Quality 3:  Only two of the standard requirements (animals, crops, and the market) implemented, and fewer than four technical concepts found.
* Quality 4: All of the standard requirements (animals, crops, and the market) implemented to an acceptable standard, with at least four of the technical concepts found to a good standard.

2. Farm merit criteria (15 marks)

* Quality 1: One or more further specific requirements implemented to an acceptable standard, or two or more to a good standard, and one or two further technical concepts found.
* Quality 2: One or more further specific requirements implemented to a good standard, and two or three further technical concepts found.
* Quality 3: One or more further specific requirements implemented to a good standard, and three or more further technical concepts found to a good standard
* Quality 4: Two or more further specific requirements implemented to a good standard, or one or more to an excellent standard, and three or more further technical concepts found to an excellent standard

3. Farm distinction criteria (15 marks) 

* Quality 1: At least one further technical concept found to an acceptable standard.
* Quality 2: At least one further technical concept found to a good standard, or two to an acceptable standard.
* Quality 3: At least three further technical concepts found to an acceptable standard, or four to a good standard, or two to an excellent standard
* Quality 4: At least four further technical concepts found to an excellent standard.

## 1. Clone down the repository and view their game

You will be provided a list of URLs of apprentices' Github Classroom repositories.

Clone your current apprentice's repo to your computer.

If you're lucky, the apprentice will have deployed their game to Netlify or similar after attending Ali's full-stack development workshop during Week 2. Hopefully you'll find a URL in their README.md where you can view their game.

If you're unlucky, you'll have to run `$ npm install` and `$ npm start` to get the webpack dev server running on your machine.

Make a note of all the specific requirements (features) they hit.

## 2. Read their own documentation of their work

Reading their timesheet will give you an indication of which of the criteria they went for. This will help you identify where to give marks. Run a `$ git log` on their repo to view their commit history. Is it legible and easy-to-follow? N.B. There are five marks available for their time sheet and git commits. 

Apprentices are allowed to collaborate with their peers, as long as they don't submit identical code. Collaboration should be noted in their time sheets. 

## 3. Run a git diff to see all their changes

There will be lots of code to sift through. The easiest way to see all their changes is to run the following command to generate a diff of their work, where XXX is the unique identifier from the Airtable record:

```
$ git diff 06dd96d4352de17aed222e78e45e71966ae64351 ':(exclude)package-lock.json' ':(exclude)client/package-lock.json' ':(exclude)yarn.lock' ':(exclude)node_modules/*' ':(exclude)client/package.json' ':(exclude)client/public/img/*' ':(exclude)package.json' ':(exclude)client/src/video/*'  ':(exclude)semantic/*'> ../diffs/XXX-diff.md
```

That commit hash is Ali's last commit hash and represents the state of the project when the apprentice accepted the assignment. You can format this `diff.md` file in your editor as Diff to make it easier to read.

You may need to add further paths for it to exclude.

Make a note of all the technical concepts they hit. The list is below. In previous marking, Ali would make a copy of this list and check each item off once he'd found evidence of it in the code. The timesheet should tell you which ones you are looking for (if apprentices write good timesheets this will make your life easier), but make sure you verfiy timesheet claims with working code in the diff.

Many of these technical requirements can be met with only a few lines of code. 

A) Full-stack development:
* DOM manipulation
* Hand-written CSS to style the Dashboard
* A CSS framework to style the Dashboard
* Refactoring the provided code base
* New tools, frameworks or approaches rather than using the given code base
* Continuous integration / continuous deployment

B) Test-driven development
* Unit testing
* Integration testing

C) Programming paradigms
* Object-oriented programming concepts including:
  * Inheritance
  * Polymorphism
  * Abstraction
  * Interfaces
* Functional programming concepts e.g. map, reduce
* Functional programming techniques in the context of a JS framework e.g.
React Hooks

D) Advanced JavaScript features
* Higher order components
* Closures
* Async/await or Promises
* Types using TypeScript
* Advanced TypeScript features such as enums
* Animating objects in P5
* Manipulation of complex data structures
* Event handling
* Routing

E) 3rd Party API Integration
* localStorage to persist state between sessions
* a database to persist data between devices
* an authentication service such as Auth0 or Firebase Auth
* the Open Weather API
* any other API

## 4. Assign marks for each section

Enter these directly into the Airtable form.  All you'll have is a GitHub username, but do watch out for conscious and unconscious bias and favouritism. Your marks will be moderated blindly to ensure consistency across all the work.

Please return a folder of labelled diffs (with the unique identifier, as above) once you have completed your marking for the moderator to review. 

## 5. Write some personalised comments

It'll only take a moment or two longer to write a couple of constructive comments, and will add enormous value for the apprentice to receive your feedback. How could they have improved their work? What did they do well? What did you enjoy or what might you have done differently? Are they making the same mistake consistently? They've put in an enormous amount of work to this project. Take a moment to give them back something useful.

Thank you and have fun!




