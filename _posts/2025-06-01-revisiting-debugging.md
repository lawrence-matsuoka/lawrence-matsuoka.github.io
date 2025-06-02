---
title: "Revisiting my Stance on Debugging"
---

I previously talked about how when debugging I mostly just print stuff and don't see much of a purpose in debuggers.
This clip from [The Standup podcast hosted by ThePrimeagen](https://youtu.be/M2ZW4uwxU8k?si=QdwGYxIGCblxPqqb&t=1342) in which Casey Muratori says that one of the main reasons he can never switch from Windows to Linux for development is because of the debuggers. He mentions specifically the Rad debugger and even Visual Studio. Fortunately the Rad debugger will eventually be ported to Linux and I will try it when it is available, but for now I will be exploring the GNU Project Debugger.

# GNU Project Debugger (gdb)

GDB being a command line tool makes it much more appealing to me. Reading through the quick Geeks by Geeks introduction, it seems that the debugger has similar features compared to what I have used in some Eclipse IDEs (they most likely have more features but I never really explored them much). I hadn't previously used the debuggers in IDEs since I prefer developing in Neovim and I am a terminal fiend. I realize now that debuggers are powerful tools and can save lots of time when running into issues. Instead of inserting random print statements everywhere, I can have breakpoints, I can view the value of local variables line-by-line, and using the gdb `tui` command I can have a somewhat nice UI.

I just wanted this post to be pretty brief and serve as a resource I can visit in the future. I will be using gdb in my next project or some other debuggers, and even if I haven't had the chance to fully explore it by my next interview, I will at least have a better answer than just saying I put print statements everywhere. 

The only specific project I have on-going is a planned game made in the Godot engine, and while I can't use gdb, I will at least be looking to have debugging as a learning outcome and to become more proficient with debuggers in general.

# References

[GDB (Step by Step Introduction)](https://www.geeksforgeeks.org/gdb-step-by-step-introduction/)

[Introduction to GDB a tutorial - Harvard CS50](https://www.youtube.com/watch?v=sCtY--xRUyI)

[CppCon 2015: Greg Law " Give me 15 minutes & I'll change your view of GDB" ](https://www.youtube.com/watch?v=PorfLSr3DDI)
