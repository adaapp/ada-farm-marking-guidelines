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

Airtable will take your mark, divide it by the number of marks available for that section, and multiply it by four (and add one) to arrive at the quality level.

It is your job to ensure the quality level matches their work.

### Section 1: Essay and UML (if you are just marking Ada Farm, please ignore this section)

1. Programming Approaches (10 marks)

* Quality 1: Incorrect reference to imperative or declarative programming paradigms. Code indicated as declarative is actually imperative, or vice versa.
* Quality 2: Definitions of an acceptable quality. Code correctly indicates different approaches but is formatted badly.
* Quality 3: Good definitions of imperative and declarative approaches with a good comparative analysis and good code examples.
* Quality 4: Excellent definitions of imperative and declarative approaches with excellent comparative analysis and code examples.

2. Programming Paradigms (10 marks)

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
* Quality 4: Excellent approach in a confident style. Faultless.

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

* Quality 1: Only one of animals, crops or the market implemented, and no further technical concepts found. 
* Quality 2: Only two of animals, crops or the market implemented, and too few technical concepts found.
* Quality 3: Only basic extension of animals, crops and the market, and not enough technical concepts found.
* Quality 4: All of animals, crops and the market implemented to an acceptable standard, with at least four of the technical concepts found.

2. Farm merit criteria (15 marks)

* Quality 1: One or more further specific requirements implemented to an acceptable standard, or two or more to a good standard, and one or two further technical concepts found.
* Quality 2: One or more further specific requirements implemented to a good standard, and two or three further technical concepts found.
* Quality 3: One or more further specific requirements implemented to a good standard, and three or more further technical concepts implemented to a good standard
* Quality 4: Two or more further specific requirements implemented to a good standard, or one or more to an excellent standard, and three or more further technical concepts found to an excellent standard

3. Farm distinction criteria (15 marks) 

* Quality 1: At least one further technical concept hit to an acceptable standard.
* Quality 2: At least one further technical concept hit to a good standard, or two to an acceptable standard.
* Quality 3: At least three further technical concepts hit to an acceptable standard, or four to a good standard, or two to an excellent standard
* Quality 4: At least four further technical concepts hit to an excellent standard.

## 1. Clone down the repository and view their game

You will be provided a list of URLs of apprentices' Github Classroom repositories.

Clone your current apprentice's repo to your computer.

If you're lucky, the apprentice will have deployed their game to Netlify or similar after attending Ali's full-stack development workshop during Week 2. Hopefully you'll find a URL in their README.md where you can view their game.

If you're unlucky, you'll have to run `$ npm install` and `$ npm start` to get the webpack dev server running on your machine.

Make a note of all the specific requirements (features) they hit.

## 2. Read their own reflection on their work

Reading their timesheet will give you an indication of which of the criteria they went for. This will help you identify where to give marks. Run a `$ git log` on their repo to view their commit history. Is it legible and easy-to-follow? N.B. There are five marks available for their time sheet and git commits. 

Apprentices are allowed to collaborate with their peers, as long as they don't submit identical code. Collaboration should be noted in their time sheets. 

## 3. Run a git diff to see all their changes

There will be lots of code to sift through. The easiest way to see all their changes is to run the following command to generate a diff of their work:

```
$ git diff 06dd96d4352de17aed222e78e45e71966ae64351 ':(exclude)package-lock.json' ':(exclude)client/package-lock.json' ':(exclude)yarn.lock' ':(exclude)node_modules/*' ':(exclude)client/package.json' ':(exclude)client/public/img/*' ':(exclude)package.json' ':(exclude)client/src/video/*'  ':(exclude)semantic/*'> diff.md
```

That commit hash is Ali's last commit hash and represents the state of the project when the apprentice accepted the assignment. You can format this `diff.md` file in your editor as Diff to make it easier to read.

Make a note of all the technical concepts they hit

## 4. Assign marks for each section

Enter these directly into the Airtable form. As ever, follow the guidelines in the Apprenticeship Lecturing Handbook. All you'll have is a GitHub username, but do watch out for conscious and unconscious bias. Your marks will be moderated to ensure consistency across all the work.

Thank you and have fun!




