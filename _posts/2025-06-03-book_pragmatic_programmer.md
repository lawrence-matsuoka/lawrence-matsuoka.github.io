---
title: "Takeaways from 'The Pragmatic Programmer' by David Thomas & Andrew Hunt"
---

A list of the topics and tips in this book. Also some quotes that I thought were profound or interesting in some way.

### Tip 1: Care About Your Craft

### Tip 2: Think! About Your Work

# 1. A Pragmatic Philosophy

## Topic 1: It's Your Life

### Tip 3: You Have Agency

## Topic 2: The Cat Ate My Source Code

### Tip 4: Provide Options, Don’t Make Lame Excuses

## Topic 3: Software Entropy

### Tip 5: Don’t Live with Broken Windows

## Topic 4: Stone Soup and Boiled Frogs

### Tip 6: Be a Catalyst for Change

### Tip 7: Remember the Big Picture

"The soldiers progressively deceive the villagers, but
the change they catalyze does them all good. However, by
progressively deceiving the frog, you’re doing it harm. Can you
determine whether you’re making stone soup or frog soup when
you try to catalyze change? Is the decision subjective or objective?"

## Topic 5: Good-Enough Software

### Tip 8: Make Quality a Requirements Issue

## Topic 6: Your Knowledge Portfolio

### Tip 9: Invest Regularly in Your Knowledge Portfolio

### Tip 10: Critically Analyze What You Read and Hear

## Topic 7: Communicate!

### Tip 11: English is Just Another Programming Language

### Tip 12: It’s Both What You Say and the Way You Say It

### Tip 13: Build Documentation In, Don’t Bolt It On

# 2. A Pragmatic Approach

## Topic 8: The Essence of Good Design

### Tip 14: Good Design Is Easier to Change Than Bad Design

ETC: Easier To Change

## Topic 9: DRY - The Evils of Duplication

### Tip 15: DRY - Don't Repeat Yourself

Applies to both code and comments. If the code is self-explanatory, then don't repeat yourself in comments.

### Tip 16: Make It Easy to Reuse

## Topic 10: Orthogonality

### Tip 17: Eliminate Effects Between Unrelated Things

## Topic 11: Reversibility

### Tip 18: There Are No Final Decisions

### Tip 19: Forgo Following Fads

## Topic 12: Tracer Bullets

### Tip 20: Use Tracer Bullets to Find the Target

## Topic 13: Prototypes and Post-it Notes

### Tip 21: Prototype to Learn

## Topic 14: Domain Languages

### Tip 22: Program Close to the Problem Domain

## Topic 15: Estimating

### Tip 23: Estimate to Avoid Surprises

### Tip 24: Iterate the Schedule with the Code

# 3. The Basic Tools

## Topic 16: The Power of Plain Text

### Tip 25: Keep Knowledge in Plain Text

The Unix Philosophy: small, sharp tools, each intended to do one thing well.

## Topic 17: Shell Games

Vindication for all the time I've spend in the terminal these past few years.

A benefit of GUIs is WYSIWYG - what you see is what you get. The disadvantage is WYSIAYG - what you see is all you get.

### Tip 26: Use the Power of Command Shells

## Topic 18: Power Editing

### Tip 27: Achieve Editor Fluency

- When editing text, move and make selections by character, word,
line, and paragraph.
- When editing code, move by various syntactic units (matching
delimiters, functions, modules, …).
- Reindent code following changes.
- Comment and uncomment blocks of code with a single command.
- Undo and redo changes.
- Split the editor window into multiple panels, and navigate between
them.
- Navigate to a particular line number.
- Sort selected lines.
- Search for both strings and regular expressions, and repeat
previous searches.
- Temporarily create multiple cursors based on a selection or on a
pattern match, and edit the text at each in parallel.
- Display compilation errors in the current project.
- Run the current project’s tests.

## Topic 19: Version Control

### Tip 28: Always Use Version Control

## Topic 20: Debugging

### Tip 29: Fix the Problem, Not the Blame

### Tip 30: Don’t Panic

### Tip 31: Failing Test Before Fixing Code

Write an automated test that reproduces the bug.

### Tip 32: Read the Damn Error Message

I quote "’nuf said."

Some additional techniques for debugging:
- Logging and/or Tracing.
- Rubber Ducking. Explain the problem to someone else.
- Process of Elimination. Determine where in the code the problem could lie (OS, compiler, application, third party product, etc.)

### Tip 33: “select” Isn’t Broken

"If you “changed only one thing’’ and the system stopped
working, that one thing was likely to be responsible, directly or
indirectly, no matter how farfetched it seems. Sometimes the
thing that changed is outside of your control: new versions of
the OS, compiler, database, or other third-party software can
wreak havoc with previously correct code. New bugs might show
up. Bugs for which you had a workaround get fixed, breaking
the workaround. APIs change, functionality changes; in short,
it’s a whole new ball game, and you must retest the system
under these new conditions. So keep a close eye on the schedule
when considering an upgrade; you may want to wait until after
the next release."

### Tip 34: Don't Assume It - Prove It

Debugging Checklist:
- Is the problem being reported a direct result of the underlying bug,
or merely a symptom?
- Is the bug really in the framework you’re using? Is it in the OS? Or
is it in your code?
- If you explained this problem in detail to a coworker, what would
you say?
- If the suspect code passes its unit tests, are the tests complete
enough? What happens if you run the tests with this data?
- Do the conditions that caused this bug exist anywhere else in the
system? Are there other bugs still in the larval stage, just waiting to
hatch?

## Topic 21: Text Manipulation

## Topic 22: Engineering Daybooks

Write stuff down because it’ll make writing your memoir easier when you’re rich and famous.

# 4. Pragmatic Paranoia

### Tip 36: You Can’t Write Perfect Software

"In a world of imperfect systems, ridiculous time scales, laughable tools, and impossible requirements, let’s play it safe." Be a defensive driver.

## Topic 23: Design by Contract

### Tip 37: Design with Contracts

Write ""lazy" code: be strict about what you will accept before you begin, and promise as little as possible in return."

## Topic 24: Dead Programs Tell No Lies

### Tip 38: Crash Early

## Topic 25: Assertive Programming

### Topic 39: Use Assertions to Prevent the Impossible

Expect (and test for) the unexpected.

## Topic 26: How to Balance Resources

### Tip 40: Finish What You Start

If malloc'd, then free it. If opening a file, remember to close it within the same function.

### Tip 41: Act Locally

## Topic 27: Don’t Outrun Your Headlights

### Tip 42: Take Small Steps - Always

### Tip 43: Avoid Fortune-Telling

# 5. Bend, or Break

## Topic 28: Decoupling

### Tip 44: Decoupled Code Is Easier to Change

### Tip 45: Tell, Don’t Ask

### Tip 46: Don’t Chain Method Calls

### Tip 47: Avoid Global Data

### Tip 48: If It’s Important Enough to Be Global, Wrap It in an API

## Topic 29: Juggling the Real World

## Topic 30: Transforming Programming

### Tip 49: Programming Is About Code, But Programs Are About Data

### Tip 50: Don't Hoard State; Pass It Around

## Topic 31: Inheritance Tax

### Tip 51: Don’t Pay Inheritance Tax

### Tip 52: Prefer Interfaces to Express Polymorphism

### Tip 53: Delegate to Services: Has-A Trumps Is-A

### Tip 54: Use Mixins to Share Functionality

## Topic 32: Configuration 

### Tip 55: Parameterize Your App Using External Configuration

# 6. Concurrency

## Topic 33: Breaking Temporal Coupling

### Tip 56: Analyze Workflow to Improve Concurrency

## Topic 34: Shared State Is Incorrect State

### Tip 57: Shared State Is Incorrect State

## Topic 35: Actors and Processes

### Tip 58: Use Actors For Concurrency Without Shared State

## Topic 36: Blackboard

### Tip 60: Use Blackboards to Coordinate Workflow

![Charlie Day meme](/assets/images/charlieday.png)

# 7. While You Are Coding

## Topic 37: Listen to Your Lizard Brain

### Tip 61: Listen to Your Inner Lizard

Allow time for passive thought.

## Topic 38: Programming by Coincidence

### Tip 62: Don’t Program by Coincidence

## Topic 39: Algorithm Speed

Big-O Notation.

### Tip 63: Estimate the Order of Your Algorithms

### Tip 64: Test Your Estimates

## Topic 40: Refactoring

### Tip 65: Refactor Early, Refactor Often

## Topic 41: Test to Code

### Tip 66: Testing Is Not About Finding Bugs

### Tip 67: A Test Is the First User of Your Code

### Tip 68: Build End-to-End, Not Top-Down or Bottom Up

### Tip 69: Design to Test

### Tip 70: Test Your Software, or Your Users Will

## Topic 42: Property-Based Testing

### Tip 71: Use Property-Based Tests to Validate Your Assumptions

## Topic 43: Stay Safe Out There

### Tip 72: Keep It Simple and Minimize Attack Surfaces

### Tip 73: Apply Security Patches Quickly

"...rely only on reliable things: well- vetted, thoroughly examined, well-maintained, frequently updated, preferably open source libraries and frameworks."

## Topic 44: Naming Things

### Tip 74: Name Well; Rename When Needed

# 8. Before the Project

## Topic 45: The Requirements Pit

### Tip 75: No One Knows Exactly What They Want

### Tip 76: Programmers Help People Understand What They Want

### Tip 77: Requirements Are Learned in a Feedback Loop

### Tip 78: Work with a User to Think Like a User

### Tip 79: Policy Is Metadata

### Tip 80: Use a Project Glossary

Define all the specific terms and vocabulary used in a project.

## Topic 46: Solving Impossible Puzzles

### Tip 81: Don’t Think Outside the Box - _Find_ the Box

## Topic 47: Working Together

### Tip 82: Don’t Go into the Code Alone

## Topic 48: The Essence of Agility

### Tip 83: Agile Is Not a Noun; Agile Is How You Do Things

# 9. Pragmatic Projects

## Topic 49: Pragmatic Teams

### Tip 84: Maintain Small, Stable Teams

### Tip 85: Schedule It to Make It Happen

### Tip 86: Organize Fully Functional Teams

## Topic 50: Coconuts Don’t Cut It

### Tip 87: Do What Works, Not What’s Fashionable

"The goal of course isn’t to “do Scrum,” “do agile,” “do Lean,” or what-have-you. The goal is to be in a position to deliver working software that gives the users some new capability at a moment’s notice."

### Tip 88: Deliver When Users Need It

## Topic 51: Pragmatic Starter Kit

### Tip 89: Use Version Control to Drive Builds, Tests, and Releases

### Tip 90: Test Early, Test Often, Test Automatically

### Tip 91: Coding Ain’t Done ’Til All the Tests Run

### Tip 92: Use Saboteurs to Test Your Testing

### Tip 93: Test State Coverage, Not Code Coverage

### Tip 94: Find Bugs Once

### Tip 95: Don’t Use Manual Procedures

Automate whatever you can.

## Topic 52: Delight Your Users

That's the point, the main purpose, le raison d'etre.

### Tip 96: Delight Users, Don’t Just Deliver Code

## Topic 53: Pride and Prejudice

### Tip 97: Sign Your Work

# 10. Postface

### Tip 98: First, Do No Harm

### Tip 99: Don’t Enable Scumbags

### Tip 100: It’s Your Life. Share it. Celebrate it. Build it. AND HAVE FUN!
