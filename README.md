<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Strong Random Password Generator
*Onur Taskin*

*Data Analytics, Barcelona 06.2019*

## Content
- [Project Description](#project-description)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

<a name="project-description"></a>

## Project Description
The aim is to build a generator that generates personlised strong random password.
In this work it is most important that the generated password is strong (in the line of later defined rules) and has a personal component, so that the individual can remember it.


<a name="workflow"></a>

## Workflow

### Define the rules

#### For the definition of passwords, two specific password-characteristics can be deduced:
    * The password has to be as complex as possible to be hard
    * The password has to be rememberable for the user

#### Rules are orientated on the recommendations of the 'German Federal Office for Information Security':
(https://www.bsi-fuer-buerger.de/BSIFB/DE/Empfehlungen/Passwoerter/passwoerter_node.html)

    * At least 8 figures
    * Use small/big letter, special characters and numbers
    * Do not use simple words that are in wordbooks or names
    * Do not simply append to the beginning or end of a password special characters like '?$%'
    * Combine words by using a special character
    * You should be able to remember it

### Implementation of the rules:
    * Password will consist of two words, which are binded through a randomly generated special character
    * User will be asked different questions to determine personalised answers
    * The answers will be rewritten in (simple) 'leetspeak' (So that the user is able to remember)
    * Due to available leetspeak-generators and dictonaries, the second word will be reversed
    * User will be acquaint with the structure of the password 

### Define questions and answers for the user
    * Two different stages for each word
    * First word(hard):
        * Choose a topic: Holidays, Countries or Subjects
            * Think of your favourite Holiday(Country or Subject). What is the first word that pops up your mind: XX
     * Second word(simple):
         * Choose a topic: Fruits, Animals or Sports
             * What is your favourite Fruit(Animal or Sport): YY
             

### Define simple leetspeak dictionary
    * Simple leetspeak dictionary with replacement of letters only by numbers
        (i=1, z=2, e=3, a=4, s=5, g=6, t=7, b=8, p=9, o=0)
        
### Define generator for random special character
    * code random

### Pseudo Code Structure

#### First stage
    * Create List: Holiday, Country, Subject
    * Create list: Fruit, Animal, Sport
    * Create Dictinary "User Answer 1" & "User Answer 2"
    * Create Dictinary "User modified Answer 1" & "User Answer 2"
    * Create Dictinary "Leetspeak"
    * Create Function: Change User Answer by Leetspeak and save in dictionary
    
#### Second stage
    * Interactive Question to user:
        * Choose a topic: Holidays, Countries or Subjects
            ONLY IF RIGHT WORD TYPED IN:
            * Think of your favourite Holiday(Country or Subject). What is the first word that pops up your mind: XX
    * Function to transform answer and save in Dictionary

    * REPEAT FOR SECOND QUESTION

    * Generate the special character between the words
    
    * Show user his true answers to the questions
    * Show user his special character
    * Show user his new password
            
<a name="organization"></a>

## Organization
How did you organize yourself? Did you use any tools?

Websites to test generated passwords : https://wiesicheristmeinpasswort.de/ and http://www.passwordmeter.com/

<a name="links"></a>

## Links
[Repository](https://github.com/Onur5/project_strong_password_generator.git) 
[Slides](https://slides.com/onurtaskin/deck/live#/)  
[Trello](https://trello.com/b/L7VnlXuh/random-number-generator)  
