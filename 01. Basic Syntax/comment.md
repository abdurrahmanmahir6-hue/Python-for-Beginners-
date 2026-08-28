# Python Comments — What They Are and Why You Should Actually Use Them

If you're just starting out with Python, you've probably already seen lines of code with a `#` in front of them, followed by some plain English text that Python seems to completely ignore. Those are comments, and once you understand what they're for, you'll wonder how you ever wrote code without them.

## So what exactly is a comment?

A comment is a line (or part of a line) in your code that Python doesn't run. It's not code — it's a note. You write it for humans, not for the computer. The interpreter skips right over it like it isn't even there.

```python
# This program calculates the area of a rectangle
length = 10
width = 5
area = length * width
print(area)
```

That first line does nothing when the program runs. Delete it, and `area` still comes out to 50. So why is it there? Because six months from now, when you (or someone else) open this file again, that one line saves you from having to re-read and mentally re-run the whole script just to remember what it does.

## The real-life version of this

Think about a recipe card. A good recipe doesn't just list "add 2 eggs" — sometimes it adds a little note in the margin like *"room temperature eggs mix better."* That note isn't a cooking step. You can't eat it. But it's the kind of thing that saves you from a mistake, or explains why a step exists in the first place.

Comments in code work the same way. The code is the recipe steps. The comment is the little note in the margin that explains the *why* behind a step, not just the *what*.

Or think of it like leaving a sticky note on the fridge for your roommate: "Don't unplug this, the wifi router is connected to it." Anyone can see the plug is there — that's obvious. What's not obvious is *why it matters*, and that's exactly the kind of thing a comment should say.

## Single-line comments

This is the one you'll use constantly. Just start the line with `#`.

```python
# Convert temperature from Celsius to Fahrenheit
celsius = 30
fahrenheit = (celsius * 9/5) + 32
```

You can also stick a comment at the end of a line of code, after the code itself:

```python
age = 25  # user's age in years
```

Both are fine. Which one you use usually just depends on whether the note applies to the whole block below it, or to that one specific line.

## What about multi-line comments?

Here's something that trips people up: Python doesn't actually have a real "block comment" feature the way some other languages do. If you want to comment out several lines, the honest way is to just put `#` in front of each one:

```python
# This function takes a list of numbers
# removes any duplicates
# and returns them sorted from smallest to largest
def clean_numbers(numbers):
    return sorted(set(numbers))
```

You'll also see people use a triple-quoted string sitting by itself as a kind of comment block:

```python
"""
This section handles user login.
It checks the password and starts a session if it's correct.
"""
```

Technically speaking, this isn't a comment at all — it's a string that Python creates and then just throws away because nothing is done with it. It works fine as a stand-in for a block comment in casual use, but it's worth knowing the difference, especially because this exact syntax has a real job elsewhere: writing docstrings, which are the official way to document what a function or class does.

```python
def calculate_area(length, width):
    """Returns the area of a rectangle given its length and width."""
    return length * width
```

That's not just a comment sitting near the function — it's attached to it, and tools like `help()` can actually read it back to you.

## Comments people actually find useful vs. ones nobody needs

Not every comment is worth writing. A comment that just repeats what the code already says clearly isn't helping anyone:

```python
# add one to x
x = x + 1
```

Anyone reading `x = x + 1` already knows it adds one to x. The comment adds nothing. Compare that to this:

```python
# Compensate for the off-by-one error in the API's page count
x = x + 1
```

Now the comment is doing real work. It's telling you *why* this strange-looking line exists, something the code by itself could never tell you. That's really the whole skill of commenting — writing down the reasoning, the context, the "trust me, this is here on purpose" — not just narrating each line back in English.

## One more everyday use: commenting code out

Sometimes you're not writing a note, you're temporarily disabling a line while you're testing something:

```python
print("Step 1 complete")
# print("debug info here")
print("Step 2 complete")
```

That middle line is still sitting there in the file, but it won't run. Developers do this constantly while figuring out what's going wrong in a program, and then either delete the line or bring it back once they're done.

## The short version

Comments don't make your program do anything different. They make your program make sense — to your future self, to a teammate, to anyone who has to read your code without you standing next to them explaining it out loud. Write them the way you'd leave a note for someone you actually care about understanding what you did, and you'll never regret having them.
