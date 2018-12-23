---
layout: post
title:      "My first CLI application and the challenges I had faced"
date:       2018-12-23 09:15:20 +0000
permalink:  my_first_cli_application_and_the_challenges_i_had_faced
---


Building my first CLI application was an overwhelming challenge, atleast that was how i looked at it before i even started. thankfully it wasnt such an erroneous challenge as i had initially percieved. I first worked out how my CLI application would function. In hindsight, it is easier to draw out your layout on paper instead of visualizing it within your mind as you will come across discrepencies whilst you are building your CLI. For example, When i was building new functionality within my CLI application. I came across a problem in which i could not go back to my previous function by my new function. I actually hadnt realized it was a problem until i ran the code several times. several times in which could have been avoided, had i planned out my CLI application on paper. 

My CLI involved a top 50 list; the list is filled with the top films of all time. The purpose of this CLI gem was for the user to look through the list of top 50 films and is then sent to a more descriptive page of the film that was searched for. This menu was filled with the title, rating, genre, a small synopsis and a URL link to find out more about the film. Again, in hindsight, i say again, its smarter and more efficient to plan things out first. I dived headfirst into creating my film object. by that i built a ton of attributes, 75% of those attributed i didnt even choose to use. I decided to make so many because i was still in the ideation phase and sort of want to get things into motion. I simplified it, the more fleshed out my CLI became and it dwindled down to 5 or 6. 

I would have to say the largest challenge was creating the scraper file. Not the syntax or even making sense of the order of things, but actually specifying the element i needed. I remember quite clearly that Ruby tends to look at scraping elements as an array of nested hashes. I remember this specifically because this was the reason why i was not recieving the correct element for my scrape. You see the problem i was running into at the time was dealing with my synopsis. It was picking up every other element because the class name was shared with most of the other elements. to overcome this challenge and after the information i had learned i realized i can specify the element more by treating the scrape as an array, and i specified it by index. 

> variable.attribute = array.method("specific element")[1].text

Another problem that i had to solve when i was building the scraper, this actually happened when i had gotten the file up and running. Nasty formatting!! it seemed as well as picking up the text for the element i was also picking up the negative space. after hefty google searching i realized the added method to get rid of negative white space was:

> variable.attribute = array.method("specific element")[1].text.strip.gsub(/\s+/,' ')

My menu changed from a visually appalling mess to an a neat and ordered list. I would have to say the largest problem i had the most was actually running my program. The thing about building a CLI within the IDE is the permissions i need with bash. This one line of code pissed me off so much that i didnt touch my project for several hours. It made me rethink my life. Here is the golden line:

> chmod +x bin/your_file

These are just a few challenges i had ran into while working on my first CLI gem. Hopefully this article will help most people so they can avoid the many frustrations i had experienced, myself. 


