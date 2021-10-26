## Pre-Work - Code 401: Advanced Javascript Development

### How to Solve Programming Problems

> When most programmers are given a programming problem in an interview, they make several key mistakes.  The most severe of those is the improper allocation of time.

> The most common mistake I see when conducting interviews or watching someone try to solve a programming problem is they try to start writing code as soon as possible.

#### A simple set of steps

1. Read the problem completely twice.
2. Solve the problem manually with 3 sets of sample data.
3. Optimize the manual steps.
4. Write the manual steps as comments or pseudo-code.
5. Replace the comments or pseudo-code with real code.
6. Optimize the real code.

> **As much as 70% of our time should be spent in steps 1-3.**

## Read the problem completely twice.

> This is the single most important step.  You may even want to read the problem 3 or 4 times.

> You want to make sure you completely understand the problem.  A good test of this is whether or not you can explain the problem to someone else.

> I cannot over-emphasize how important this step is!

> If you don’t understand the problem, you cannot solve it.  Do not worry about wasting time here, because the better you understand the problem, the easier it will be to solve it.

> If you are given any examples along with the problem, make sure you have worked through the examples and understand why the answers are correct for each one.

If I give you a string “Zebra”, and ask you to reverse it, most people will do the following manual steps.
+ Write “Zebra” down.
+ Start a new word, and put “a” as the first letter.  (Why –> because it is the last letter, we want to start here)
+ Put “r” down as the 2nd letter.  (Why –> because it is the next letter backwards from the last letter we copied)
+ Put “b” down as the 3rd letter.  (Why –> same as above)
+ Etc

## Optimize the manual solution

People often don’t realize how valuable this step is.  It is much easier to rearrange and reconstruct and idea or algorithm in your head than it is in code.

It’s well worth the effort to try and optimize the actual solution or simplify it when it is still in the most easily malleable state.

What you want to do here is figure out if there is another way you can solve the problem easier, or if there are some steps you can cut our or simplify.

Let’s look at our string reversal example and see if we can simplify the steps.

We should be able to immediately recognize that we can use a loop here to reduce the manual steps.  Our duplicate why’s for most of our steps tell us that we are doing the same thing over and over for each step, just with different data.

1. Write “Zebra” down.
2. Start at the last letter in the word and create a new empty word.
3. Append the current letter to the new word
4. If there is a previous letter, make the previous letter the current letter and start back at 3.
Look how close we are getting to code at this point.  You should be tempted to actually write the code for this.  That is good, it tells you that you have solved and simplified the problem well.  Writing code should now become very easy.

## Write pseudo-code or comments

> Many times you can skip this step if you have a really good handle on the problem or your previous steps already created a detailed enough description of the solution that coding it is already a 1 to 1 translation.

```
/ NewWord = “”

// Loop backwards through word to reverse

//   NewWord += CurrentLetter

// Return NewWord
```

## Replace comments with real code

> This step should be extremely easy at this point.  If you have done all the other steps, this step involves no problem solving at all.

```
String newWord =""
for(int index = oldWord.Length – 1; index <= 0; index—)
   newWord += oldWord[index];
return newWord;
```

If you don’t know your programming language well enough to do the translation, you may need to brush up here on some basic constructs.  Any language you expect to be able to solve algorithm type problems in, you should know how to do the following things:

+ Create a list
+ Sort a list or array
+ Create a map or dictionary
+ Loop through a list, or dictionary
+ Parse strings
+ Convert from string to int, int to string, etc

## Optimize the real code

Sometimes this step isn’t necessary, but it’s worth taking a look at your code and figuring out if you can cut out a few lines or do something simpler.

This is also a good place to make sure all your variables are named with long meaningful names.  I cannot stress enough how important having good names for your variables and methods is for helping the person evaluating your code to understand what you were trying to do.  This is especially important when you make a mistake!

*** 

> “Pretend your time is worth $1,000/hr. Would you spend five of them doing extra work for free? Would you waste one on being angry?” -
Niklas Göke

Still, many people waste much of their time on pointless, low-quality activities that don’t help them reach their true goals — their mission.
The truth is, most people value their time at far, far less than it’s worth.
They say yes to things they have no business doing. They give away their talents, attention, and effort to others who take, take, take.
They spend hours watching low-quality television and social media when they should be productive and effective.

### But what if you placed a high value on your time?

+ How would that change you? Your life? Your family? Your future?
+ Imagine that an hour of your time is worth $1,000.
+ What would your life look like?
+ What people would you stop putting up with?
+ What problems would you stop wasting time on?
+ What things would you stop — and start — doing?

> “Most people have no clue what they are doing with their time but still complain that they don’t have enough.” -Grant Cardone, NYT best-selling author

> “Busyness” Isn’t a Badge of Honor; It’s a Sign of Weakness

> “People think focus means saying yes to the thing you’ve got to focus on. But that’s not what it means at all. It means saying no to the hundred other good ideas that there are. You have to pick carefully. I’m actually as proud of the things we haven’t done as the things I have done. Innovation is saying no to 1,000 things.”

***

![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200326191711/How-to-Think-Like-a-Programmer.png)

+ If you’re interested in programming, you may well have seen this quote before:

> “Everyone in this country should learn to program a computer, because it teaches you to think.” — Steve Jobs
You probably also wondered what does it mean, exactly, to think like a programmer? And how do you do it??

Essentially, it’s all about a more effective way for problem solving.

In this post, my goal is to teach you that way.

By the end of it, you’ll know exactly what steps to take to be a better problem-solver.

**Why is this important?**

We all have problems. Big and small. How we deal with them is sometimes, well…pretty random.

Unless you have a system, this is probably how you “solve” problems (which is what I did when I started coding):

1. Try a solution.
2. If that doesn’t work, try another one.
3. If that doesn’t work, repeat step 2 until you luck out.
Look, sometimes you luck out. But that is the worst way to solve problems! And it’s a huge, huge waste of time.

![](https://i.pinimg.com/originals/7e/35/5e/7e355e71847d741e540da3404662794f.png)

**1. Understand**

> Know exactly what is being asked. Most hard problems are hard because you don’t understand them (hence why this is the first step).

**2. Plan**

Don’t dive right into solving without a plan (and somehow hope you can muddle your way through). Plan your solution!

Nothing can help you if you can’t write down the exact steps.

In programming, this means don’t start hacking straight away. Give your brain time to analyze the problem and process the information.

**3. Divide**

Pay attention. This is the most important step of all.

Do not try to solve one big problem. You will cry.

Instead, break it into sub-problems. These sub-problems are much easier to solve.

Then, solve each sub-problem one by one. Begin with the simplest. Simplest means you know the answer (or are closer to that answer).

After that, simplest means this sub-problem being solved doesn’t depend on others being solved.

> “If I could teach every beginning programmer one problem-solving skill, it would be the ‘reduce the problem technique.’

> For example, suppose you’re a new programmer and you’re asked to write a program that reads ten numbers and figures out which number is the third highest. For a brand-new programmer, that can be a tough assignment, even though it only requires basic programming syntax.

> If you’re stuck, you should reduce the problem to something simpler. Instead of the third-highest number, what about finding the highest overall? Still too tough? What about finding the largest of just three numbers? Or the larger of two?

**4. Stuck?**

By now, you’re probably sitting there thinking “Hey Richard... That’s cool and all, but what if I’m stuck and can’t even solve a sub-problem??”

First off, take a deep breath. Second, that’s fair.

Don’t worry though, friend. This happens to everyone!

The difference is the best programmers/problem-solvers are more curious about bugs/errors than irritated.

> + Debug: Go step by step through your solution trying to find where you went wrong. Programmers call this debugging (in fact, this is all a debugger does).

>“The art of debugging is figuring out what you really told your program to do rather than what you thought you told it to do.”” — Andrew Singer

>Reassess: Take a step back. Look at the problem from another perspective. Is there anything that can be abstracted to a more general approach?

>“Sometimes we get so lost in the details of a problem that we overlook general principles that would solve the problem at a more general level. […]

**Practice**

Don’t expect to be great after just one week. If you want to be a good problem-solver, solve a lot of problems!

Practice. Practice. Practice. It’ll only be a matter of time before you recognize that “this problem could easily be solved with <insert concept here>.”

How to practice? There are options out the wazoo!

Chess puzzles, math problems, Sudoku, Go, Monopoly, video-games, cryptokitties, bla… bla… bla….

***
## How to Use the 5 Whys

1. Assemble a Team
Gather together people who are familiar with the specifics of the problem, and with the process that you're trying to fix. Include someone to act as a facilitator , who can keep the team focused on identifying effective counter-measures.

2. Define the Problem
If you can, observe the problem in action. Discuss it with your team and write a brief, clear problem statement that you all agree on. For example, "Team A isn't meeting its response time targets" or "Software release B resulted in too many rollback failures."

Then, write your statement on a whiteboard or sticky note, leaving enough space around it to add your answers to the repeated question, "Why?"

3. Ask the First "Why?"
Ask your team why the problem is occurring. (For example, "Why isn't Team A meeting its response time targets?")

Asking "Why?" sounds simple, but answering it requires serious thought. Search for answers that are grounded in fact: they must be accounts of things that have actually happened, not guesses at what might have happened.

This prevents 5 Whys from becoming just a process of deductive reasoning, which can generate a large number of possible causes and, sometimes, create more confusion as you chase down hypothetical problems.

4. Ask "Why?" Four More Times
For each of the answers that you generated in Step 3, ask four further "whys" in succession. Each time, frame the question in response to the answer you've just recorded.

![](https://www.mindtools.com/media/Diagrams/5_Whys_Figure_1_Single_Lane.jpg)

![](https://www.mindtools.com/media/Diagrams/5_Whys_Figure_2_multiple_lanes.jpg)

5. Know When to Stop

You'll know that you've revealed the root cause of the problem when asking "why" produces no more useful responses, and you can go no further. An appropriate counter-measure or process change should then become evident. (As we said earlier, if you're not sure that you've uncovered the real root cause, consider using a more in-depth problem-solving technique like Cause and Effect Analysis , Root Cause Analysis , or FMEA .)

6. Address the Root Cause(s)

Now that you've identified at least one root cause, you need to discuss and agree on the counter-measures that will prevent the problem from recurring.

7. Monitor Your Measures

Keep a close watch on how effectively your counter-measures eliminate or minimize the initial problem. You may need to amend them, or replace them entirely. If this happens, it's a good idea to repeat the 5 Whys process to ensure that you've identified the correct root cause.