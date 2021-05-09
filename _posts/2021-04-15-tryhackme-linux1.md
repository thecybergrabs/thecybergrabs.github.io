---
layout: post
title: TryHackMe - Linux Fundamentals Part 1 Walkthrough
color: orange
tags: [Try Hack Me, Writeup, Linux]
---

Welcome to [Linux Fundamentals Part 1](https://tryhackme.com/room/linux1) on [TRYHACKME](https://tryhackme.com/room/linux1)
In this series of Linux Fundamentals, we’ll introduce you to bash (the standard Linux shell) and how to take full advantage of standard Linux commands like ls, cp, and mv, explain inodes and hard and symbolic links, and much more.

By the end of this series (Linux Fundamentals Part 1,2,3),you’ll have a solid grounding in Linux fundamentals and commands.
This tutorial is ideal for those who are new to Linux or those who want to improve their understanding of fundamental Linux concepts. For the beginners, much of the materials will be new, but the experienced Linux users may find this tutorial to be a great way of rounding out their fundamental Linux skills.

Lets go ahead and deploy the machine and then we will see out first task what does it say.

**Task 1 : Intro**
{% include aligner.html images="linux1/1.jpg" column=1 %}
{% include aligner.html images="linux1/2.jpg" column=1 %}

If you want to SSH into the machine than

> _Username : shiba1 Password : shiba1_

{% include aligner.html images="linux1/3.jpg" column=1 %}

1. Read the above.
> _No answer needed._

2. Deploy the machine attached to this task!
> _No answer needed._

**Task 3 : Basic Command Execution**
{% include aligner.html images="linux1/4.jpg" column=1 %}
1. Read the above.
> _No answer needed._

**Task 4 : [Section 2: Running Commands] — Manual Pages and Flags**
1. How would you output hello without a newline?
> _echo -n hello_

**Task 5 : [Section 3: Basic File Operations] — ls**
{% include aligner.html images="linux1/5.jpg" column=1 %}
1. What flag outputs all entries
> _-a_

2. What flag outputs things in a ”long list” format
> _-l_

**Task 6 : [Section 3: Basic File Operations] — cat**
{% include aligner.html images="linux1/6.jpg" column=1 %}
1. What flag numbers all outputs all lines ?
> _-n_

**Task 7 : [Section 3: Basic File Operations] — touch**
{% include aligner.html images="linux1/7.jpg" column=1 %}
1. Read the above!
No Answers needed

**Task 8 : [Section 3: Basic File Operations] — Running A Binary**
1. How would you run a binary called hello using the directory shortcut ?
> _./hello_

2. How would you run a binary called hello in your home directory using the shortcut ?
> _~/hello_

3. How would you run a binary called hello in the previous directory using the shortcut ?
> _../hello_

**Task 9 : Binary — Shiba1**
Now that you’ve learned basic file operations, you can solve the first challenge! This challenge is pretty simple, create a file called noot.txt.
Once you’re done run the binary and you’ll be given the password for the user shiba2!
{% include aligner.html images="linux1/8.jpg" column=1 %}
1. What’s the password for shiba2 ?
> _pinguftw_

**Task 10 : su**
Now that we have our next user password, it seems like a good time to cover su. su is a command that allows you to change the user, without logging out and logging back in again. For example if you wanted to switch to shiba2 while you’re the user shiba1, you would type su shiba2 . You would then be prompted for a password and if you entered shiba2’s password you would then become shiba2
> _su shiba2_

1. How do you specify which shell is used when you login?
> _-s_

**Task 11 : Linux Fundamentals 2**
1. Join the Linux Fundamentals 2 room and continue your learning journey: https://tryhackme.com/room/linux2
> _No answer needed_

Now that you have some beginner knowledge of using Linux, it’s time you take it a step further and join the Linux Fundamentals 2 room. Stayed tuned for Linux Fundamentals Series. Till then goodbye and Happy Hacking.

[Aditya Trivedi](https://www.linkedin.com/in/aditya-trivedi-2021)
