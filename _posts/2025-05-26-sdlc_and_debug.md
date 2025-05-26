---
title: "The Software Development Life Cycle and Debugging"
---

It seems in the two interviews I have managed to secure, I got absolutely roasted and toasted by questions related to these subjects so I am defining them here and trying to apply the terminology with what I did on my own personal projects to solidify my shame and regret in not knowing this earlier (no matter how much I feel like knowing these terms won't make me a better programmer).

# The Software Development Life Cycle (SDLC)

The Software Development Life Cycle is a step-by-step methodology to develop, maintain, replace, and improve quality software. Unknowingly, I have used these steps in creating many of my projects, but never defined these steps as being something I need to know the terminology for, rather as something I just thought about and did. 

I wanted to make this blog post to formally define what the SDLC is and how I've used it in my own projects. Since I didn't know the specific steps when asked in interviews, I would always respond with what was effectively an "I don't know". 

After the first interview going through that, I did review the SDLC, but the terms are still new to me and memorization has never been my strong suit. In my second interview where I was asked about this, I actually did remember one step, testing, which I asked this clarifying question: "Sorry I can't quite place it in my mind, an example would be testing, wouldn't it?", to which I got the response from the interviewer "I'm the one asking questions here". 

That definitely soured my experience and took my mind out of it for the rest of the interview. But because of that experience and probably a bit of spite, I want to leave this post here for my own future reference.

## Planning

The first stage of the SDLC, planning. Typically this is done by analyzing the market. Since most of my projects are out of enjoyment, rather than finding gaps in the market, this is definitely the stage where I have the least experience. At least with [XtI](), a command-line tool made for chemists, my friend Nick had identified that too much of chemists' time was spent writing boilerplate when it should be an automated process to submit jobs for chemistry computation. We also recognized that chemists don't have any typical development environment and that the program should be usable on Windows, MacOS, and Linux, which is why for input handling we used C and that users would only need to install Lua to ensure that the scripts performing file transformations can run. 

If I were to use [HexFML]() as an example, there is no "need" for a game, but in my brief research I did notice that there was a lack of multiplayer online versions of the game Hex. While my main priority in writing the game was to get some experience with C++, I also made a game that mathematicians and others interested in Hex could now play online from the comfort of their home (or at least they will be able to once I decide to release the game and finish the 1% of it I would like to finish).

## Defining

Here, we define the requirements of the software. Meaning that we consult with people who will use the software and market research to determine what functionality the software will have, what technology will we use, and what the software will do. 

For Mastodon Studios, we are currently in this stage for the planned horror game we are making. I created a Game Design Document (GDD) template where we have discussed but still need to formalize the gameplay and the various features. I also informally did this when making HexFML, where I knew that I wanted to have online multiplayer.

## Designing

During the design phase, the best approach to the software architecture is determined. Multiple designs are presented and the best is chosen to continue into the next stage. For the horror game, we have a Technical Design Document (TDD), which I need to finish writing, where we are formalizing the software architecture and know what needs to be completed. When choosing the best approach to multiplayer for HexFML, I chose between Peer-to-peer and hosting a server. P2P was probably the best for my use case since I would not have to front server costs, and the game is for two players so it made sense to have the players connect directory to each other over TCP sockets. 

## Development

We move onto the development phase, the fun part for me. We follow the conventions, style guide, design choices, and protocols set by the previous phase. Version control and code review are also a part of the development phase. I use version control and have written guidelines that we will use at Mastodon Studios for version control, but I have never participated in a format code review. This is something I really wish to in an actual job, also with open source software I can't wait to get absolutely ripped apart whenever I get to contributing to one of those projects.

## Testing

Testing is and should be done throughout the SDLC (i.e. with unit/integration tests during the development phase), but in this phase there is a focus on tracking flaws and improving the quality. When writing HexFML, I did a lot of manual testing of the game. Playing against myself, seeing if I got the correct win screens, the gameplay was smooth, or if I had any crashes from memory leaks. 

## Deployment

In this final stage, the software is released. Feedback is taken and maintenance is done. I guess alongside planning, I haven't really encountered this stage since I have not yet deployed software that has been used. I will be getting feedback soon for XtI and hopefully will be one day for HexFML as well. 

# Debugging

Another interview question that crosses me up is about debugging. I feel like my answers are not terrible when it comes to debugging, but the interviewers never seem quite satisfied so I'm going to dive a bit deeper into this question. 

## Print or log

In simple systems, it is possible to write some print functions into the code to understand the code execution and what is happening. I used this a lot in debugging HexFML, but I don't think this would really work in more complicated code bases. The largest code base I've worked on was HexFML which had about 3,000 lines of code. In a production environment with orders of magnitude larger lines of code, print debugging may be a bit difficult to be done. 

## Breakpoints and step-through

I have used this in embedded systems development since I am somewhat forced into using an IDE instead of using Neovim like I usually do. 

## Reflection

I don't know, I feel like I understand how to debug code, I just have difficulty in communicating that (reoccurring theme). For future reference to myself, I should say something along these lines when asked: "If I encounter a bug, my first step is to reproduce the problem and determine what the source could be. For example, while making HexFML I had a boolean that kept track of which player would go first in multiplayer matches which was in the Peer class. The problem was that sometimes the game would determine that both players had the same move (i.e. both were going first), which broke the game. Firstly, I isolated the problem to either the Peer class, or the OnlineGame class where the Peer class was being called. There I could print out the value of the boolean goesFirst. What the expected outcome is that the host randomizes who goes first, and sets their boolean to true if they are first, false if they are not. The opposite value is then sent to the client. The OnlineGame class then takes the values from both host and client and assigns them their determined side. I looked at the Peer host and client logic to ensure that the values were being assigned correctly, and could see that the problem must lie with the OnlineGame class. The issue was instead of referencing the Peer class with `Peer &peer`, I was creating a new instance with `Peer peer`, so the value was not sent appropriately to the other player. This is why sometimes the game would work correcly and sometimes the game would break."

I definitely do not have experience debugging in a complex system, but I believe that I have good logical thinking and understanding of the order in which things are called which helps me to write code where I avoid a lot of bugs. But maybe this is just my overconfidence speaking. If only some company would give me a job and take me down a peg.
