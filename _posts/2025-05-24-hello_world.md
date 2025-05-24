---
title: "Hello, World!... or Blinky?"
---

This is my first blog post that will serve many purposes, both technically and personally. I aim to primarily use this as a technical blog to keep a track record of what I have learned and accomplished. Writing these ideas and thoughts down will serve as a useful way of better learning how to communicate more challenging concepts, whether in math, programming, or other areas I want to learn. On a personal level, I think it might be interesting to break some of these posts up with more "random" ideas, such as books I'm reading, how my weightlifting training is going, or some other miscellaneous things.

For some background, I am about to complete my Bachelor's of Science in Mathematics with a minor in Business. I have lots of fun learning and solving problem in certain math topics (like number theory, combinatorial game theory, or discrete math), and I like learning about low level programming and how the computers we use function. In this post, I'll be reflecting on how I got to this point, and hopefully to clear up for myself what I want to pursue in the future. I'm a bit confused at this point since I'm having difficulty finding a job and doubting myself and my interests because of this. It seems like a good idea to write this reflection and start a blog to document what I learn so I don't forget.

## Booting up

I have always loved putting things together. When I was a kid, I built lego and model kits obsessively. Never because I enjoyed looking at them or having them, but because the process of piecing them together was all I cared about. This naturally transitioned into the first time I had my own computer when I was 12 years old, a PC where I chose all the individual parts. My dad and I stayed up until 2AM the night all the parts arrived and I used this PC until I was 21 and moved out of my parents' home into an apartment.

During those 9 years I should have realized earlier that technology was an area I should study and actually work in, instead of dedicating my life to gaming. My parents had an expectation that I would go straight into university from high school and when looking back it would be obvious that I hadn't had much foresight at all. I decided to apply and pursue a Bachelor of Commerce because I wasn't too sure what to do, and because my brother had by this time established a very successful career in finance on Bay Street. It took me 2.5 years pursuing a degree in accounting to realize that maybe this wasn't quite the right field for me. The most useful thing to come out of my business degree was landing several internships and working for my first good boss, David, at his startup. I came in as a business student and left as a statistics student (which did not stick for very long before I made the pivot into mathematics). Working made me realize that what I enjoyed most from business was the "technical" aspects. Things like using Excel and PowerPoint, while I dread networking and making connections. This isn't about meeting new people but it's the feeling of making surface-level and transactional relationships that I really do not like, but that's a whole other can of worms.

## Loading...

Basically to sum up, all of my past experience has made me who I am today and have led me to my current interests. Enough about me and onto the actual goals of the block now. Primarily, I want to document my exploration of more subjects in mathematics and computers, both software or hardware.

### Mathematics

I want to improve my calculus and take real analysis a bit more seriously. I think I also should brush up on my linear algebra since it seems to be one of the most applicable fields of mathematics for programming. This is also to lay a solid foundation for diving into abstract algebra, which I wish I had taken classes in since the very brief topics we touched on in my cryptography class were very interesting. And speaking about cryptography, that class is easily my favourite "applied" math course I took throughout my degree. I care about security and privacy which is why I self-host many services, and also am interested in careers in security whether it be more of the security research route of the cryptography route.

### Lower level programming

I won't claim that I am a "good" C programmer, but I will say that in terms of programming languages, C has proven to be my one true love. I will always think that writing code in C is both fun and understandable. Because the capabilities of the language are so simple and there is very little abstraction, everything seems so clear while writing C. Of course, it's difficult to write C safely and I'm sure I make many mistakes but throughout the process I always have fun with it. I wrote a bit of C++, mostly when making the game [HexFML](), and I can see the appeal but the language seems like such a mess to me in so many ways. I will start using C++ more, since I know it is quite an employable language (and for me more enjoyable than many others).

Assembly is something I've chipped away at for a while but can never get too invested in since there are basically no jobs that care if you can write Assembly. I have written simple programs on an MSP430 though and also wrote a bootable OS that prints out "Hello World" in x86 Assembly using NASM and QEMU. I want to eventually write a fully fledged operating system to automate the future garden and home that my girlfriend and I want to own in the future. If you have ever played Stardew Valley, the inspiration is the farm computer item from that game.

## Buffering

This brings us up to speed with the present. Now as a graduate, I am on the job hunt and it's proven to be a bit more challenging than I expected. I've narrowed down my path moving forward to the areas listed below, and with some I am making compromises on what actually interests me and what interests me enough.

### Cryptography

Number theory was my favourite subject to learn about, and I also enjoy mathematical history. Naturally, cryptography would end up being one of my favourite classes together with number theory. Any job involving cryptography seems pretty fun, whether implementation or research. However, there are not many opportunities, especially since what is probably the #1 employer of cryptographers/cryptanalysts is the Communication Security Establishment (CSE) which only has offices in Ottawa. There are some remote opportunities working for cryptocurrency centered companies and it seems that the Go programming language is fairly popular with these job postings. Based on what I have read, this is because Go has fairly robust and featureful standard cryptography libraries.

To learn more about cryptography (especially implementation), I am now reading "Applied Cryptography" by Bruce Schneier. I also plan to complete the [Cryptopals crypto challenges](https://cryptopals.com) either in C, Assembly (x86, ARM, or RISC-V), or Go. I would have to learn more Assembly, and basically learn all of Go, but I think both could prove somewhat useful for future career and projects.

This path would satisfy my desire for mathematical problems and low level programming. The main issue I see is the lack of opportunities, especially for undergraduate students. I may have to go to grad school to develop my mathematical abilities further, but that is not exactly what I'd like to do at this moment.

### Embedded systems and firmware

I enjoy messing around with hardware. It's fun to wire circuits, and solder, and mess around with microcontrollers. I've made basic things with Arduinos, STM32s, and MSP430s. I also have an ESP32 and Raspberry Pi if I ever wanted to get into the embedded Linux space. And math is an important skill when working on Digital Signal Processing (DSP). Another way for me to combine math and low level programming since most of the programming in embedded is in either C, C++, or Assembly. The only issue is that I need a significant more practice and project work accomplished to secure a job.

### Software development

Software development is easily the most abundant in job opportunities. Since starting my job search, I've identified a few course corrections I needed as a math student competing against computer science students. I read through "Grokking Algorithms" by Aditya Bhargava so I could better apply my math foundation in explaining how I know what data structures and algorithms are. I plan to quickly go through "A Tour of C++" by the man himself, Bjarne Stroustrup, since the overlap between languages I'd like to use and languages jobs ask for basically involves only C++. I do use Python, but it's not my favourite to work with, and I am definitely not a webdev and have rarely used JavaScript/TypeScript, though I have professionally used JavaScript in an internship funnily enough.
Added to the reading list are "The Pragmatic Programmer" by David Thomas and Andrew Hunt, "Cracking the Coding Interview" by Gayle Laakmann McDowell, and many other books that will help in becoming a better software develop and programmer in general.
I have some gripes with software development as work and a career that I won't go into (please hire me if you're reading this potential future employers), but I will not deny that this career path would be great for skill development and I could always transition into the other paths after working as a software dev. And there's no denying that this would be a technically satisfying career.

### IT and cybersecurity

I wouldn't mind doing help desk, but the real goal would be reverse engineer/threat intelligence/malware analyst/security researcher sort of position. Things where at least knowing low level code would be useful, with the caveat that being able to read it is significantly more important than being able to write it. I have the book "Practical Malware Analysis" by Michael Sikorski on my reading list and I have gone down the rabbit hole to explore a bit, but I think I would miss actually writing code that isn't just scripts. But security is something I care about and I could see myself feeling a lot of value from a career like this. Ideally a combination of discovering the vulnerabilities and writing the patches brings me a mix of this and cryptography would be an exciting opportunity.

### Game development

Another possibility in the distant future may be in game development. I am currently working on a project with my girlfriend and our friend where we are planning on making a horror game in Godot. I have a bit of experience with gamedev in the aforementioned HexFML, and this could definitely be an interesting and satisfying career path if I'm able to develop closer to the hardware. As it currently stands, I see gamedev as more of a creative outlet than anything.

The above are all my current options, and I'm still not quite certain which path I will lean towards.

## Shutting down

I appreciate anyone who has read through this post. I hope to have a somewhat regular posting schedule in the future and accomplish lots of learning during this time.
