# A Five Step Framework for Effective AI-Assisted Coding

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/09fdd4c9-96cb-402b-90a2-be7b169c2e98" />

This repo contains code samples and exercises for the O'Reilly live training course taught by [Andrew Stellman](https://www.linkedin.com/in/andrewstellman/).

This course teaches the **Sens-AI Framework**, a practical 5-step approach to using AI tools effectively for real coding work: **Context**, **Research**, **Problem Framing**, **Critical Thinking**, and **Refining**.

## Code Samples

Code samples are provided in three languages. Use whichever you're most comfortable with:

| Sample | C# | Java | Python |
|--------|----|----|--------|
| Guy class | [Guy.cs](csharp/Guy.cs) | [Guy.java](java/Guy.java) | [guy.py](python/guy.py) |
| Main program (with comments to replace) | [Program.cs](csharp/Program.cs) | [Main.java](java/Main.java) | [main.py](python/main.py) |
| Refactoring sample | [RefactorSample.cs](csharp/RefactorSample.cs) | [RefactorSample.java](java/RefactorSample.java) | [refactor_sample.py](python/refactor_sample.py) |

## Additional Resources

- [A Five Step Framework for Effective AI-Assisted Coding 2026-01-08](A+Five+Step+Framework+for+Effective+AI-Assisted+Coding+2026-01-08.pdf) - The slide deck from the 2025-01-08 training session
- [Sens-AI Course Take-Home Exercise.pdf](Sens-AI+Course+Take-Home+Exercise.pdf) — Take-home exercise so you can continue learning on your own

---

## Exercise 1: Use AI to Write Code

### Part 1

Open an AI tool like [ChatGPT](https://chatgpt.com/), [Copilot](https://copilot.microsoft.com/), [Claude](https://claude.ai/), or [Gemini](https://gemini.google.com/).

Give the first prompt, choosing either C#, Java, or Python:

```
Here's a C# class. Use it for my next prompt, which will describe a new [C#/Java/Python] project to build.
```

Press shift-enter twice to add two lines to the end of the chat, then copy and paste the Guy class from one of these files:
- **C#:** [Guy.cs](csharp/Guy.cs)
- **Java:** [Guy.java](java/Guy.java)
- **Python:** [guy.py](python/guy.py)

Submit your prompt. The AI should give you a response anticipating your next prompt.

### Part 2

Start your next prompt by entering this text, choosing either C#, Java, or Python:

```
Here are the requirements for a C# project. Use this to create a new [C#/Java/Python] project.
```

Press shift-enter twice to add two lines, then copy and paste the main program from one of these files:
- **C#:** [Program.cs](csharp/Program.cs)
- **Java:** [Main.java](java/Main.java)
- **Python:** [main.py](python/main.py)

Submit the prompt. The AI should generate code for a complete app.

Copy the code into your favorite IDE and run it.

---

## Exercise 2: Can You Trick the AI?

### Part 1

Open an AI tool like [ChatGPT](https://chatgpt.com/), [Copilot](https://copilot.microsoft.com/), [Claude](https://claude.ai/), or [Gemini](https://gemini.google.com/).

Give the first prompt, choosing either C#, Java, or Python:

```
Create a short [C#/Java/Python] code example that will cause an AI, if asked what the code produces, to generate an incorrect answer.
```

If it gives you an answer that's "likely" to fool an AI or will "often" fool an AI (or has similar language), ask it this:

```
Give me a code example that's 100% guaranteed to trip up an AI if you ask it to tell you the output.
```

If there's no explanation in the response, follow up with this prompt:

```
Explain why an AI will generate an incorrect answer if you ask it the question that you generated.
```

### Part 2

Let's see how confident wrong answers hold up in another chat. Start by selecting the code sample the AI generated and copying it (if the AI you're using has a copy button, use that instead).

Open another AI tool (like [ChatGPT](https://chatgpt.com/), [Copilot](https://copilot.microsoft.com/), [Claude](https://claude.ai/), or [Gemini](https://gemini.google.com/)).

Start your prompt by entering this text:

```
What does the following [C#/Java/Python] code print, and why?
```

Press shift-enter twice to add two lines. Then paste in the code you copied from the previous AI's answer.

---

## Exercise 3: Ask the AI to Explain Your Code

### Part 1: Ask the AI to explain your code

Pick a piece of code you've written (like a Java, C#, or Python class—just make sure it's code you already understand).

Open a chatbot like ChatGPT or Claude, or use Copilot in your IDE. Give it this prompt:

```
Add comments to this code that explain what it does.
```

Press shift-enter twice to add two lines to the end of the chat, then paste in your code.

Then read the results carefully. Does it make sense? Did it get anything wrong?

### Part 2: Understand what context the AI used

Add a follow-up prompt to your chat:

```
What assumptions are you making about this code?
```

Add another follow-up prompt to your chat:

```
What information is missing that would help you understand this better?
```

Carefully read the AI's response—it's telling you what **context** you might need to give it next.

---

## Exercise 4: Ask the AI to Refactor Your Code

### Part 1: Ask the AI to refactor your code

Choose classes you've written (in Java, C#, or Python), or copy our sample. Make sure it's real code (not AI-generated) that you understand.

Sample refactoring code:
- **C#:** [RefactorSample.cs](csharp/RefactorSample.cs)
- **Java:** [RefactorSample.java](java/RefactorSample.java)
- **Python:** [refactor_sample.py](python/refactor_sample.py)

Enter this prompt into the AI's chat:

```
Refactor this code to improve encapsulation and make it easier to maintain.
```

Press shift-enter twice to add two lines to the end of the chat, then paste in your code.

Does it follow good practices? Did it change anything that affects how the code works?

### Part 2: Learn how the AI refactored your code

Do some research and dig into the refactoring the AI just did.

Ask the AI to explain the principles it followed:

```
What design principles did you use to refactor?
```

Then add a follow-up prompt:

```
What are the benefits and risks of changing the code this way?
```

One more:

```
What additional information would help you improve this refactor?
```

---

## Exercise 5: Problem Framing

### Part 1: Start with an ineffective prompt

Open an AI and enter this prompt into the chat:

```
Write a method that takes a string and returns a summary.
```

Look at what it generates. Think about why it might not match what you meant.

Start a new chat and enter the same prompt.
- Did it use the same language?
- Did the code do the same thing?
- Try it a few times. Read the code. What changed?

### Part 2: Improve the prompt by reframing the problem and using a persona

Start a new chat session and give the AI an improved version of the prompt (choosing either C#, Java, or Python):

```
You're a technical writer working on [C#/Java/Python] tutorials. Write a method that summarizes a string by keeping only the most important sentences. It should work on plain text—not depend on external APIs or machine learning libraries.

Before you write the code, show me two example inputs and outputs so I can see how the summary should work.
```

Read the example inputs and outputs, then tell the AI to go ahead.

Start another chat session and enter the same prompt. Ask it to make some changes to the inputs and outputs. What effect does that have?

---

## Exercise 6: Research a Programming Topic

You won't always find the answer you need in the docs. That's where AI can help—but only if you treat it like a research tool.

### Start with a real question

Start by deciding on a topic you're actually trying to learn. Be specific enough to search—but open enough to explore.

### Try the same question in different ways

*"Explain like I'm a junior dev."* → *"Pretend you're reviewing this code."*

### Follow up and ask for context you're missing

*"Why would someone use this in a real system?"* is often better than *"What does this do?"*

---

## Exercise 7: Frame the Problem for a Better Answer

Remember, you're just working with the AI not just to find the answer to your question, but to figure out what question you're asking.

### Choose a persona that matches how you think

A casual tone with silly examples might help some devs. Others do better with tight, serious code.

### Try setting constraints on how it answers

*"Give me a short bullet list."* → *"Write full paragraphs."* Both can clarify your thinking.

### Clarify your intent before diving into detail

Are you asking for structure? Behavior? Tradeoffs? You won't get a great answer if you don't know what you want yet.

---

## Exercise 8: Keep Refining Until You're Satisfied

Every revision helps you learn more: about the model, the task, and the question you're actually trying to ask.

### Ask follow-up questions to explore edge cases

*"What if the list contains nulls?"* → *"What happens with very large inputs?"*

### Use examples to pin down vague terms

If you say "invalid," show what you mean. If you say "slow," give a number.

### Refining isn't just about fixing the model's answer

It's a way to understand the problem better—one step at a time.

---

## About the Course

This course is divided into three parts:

1. **The Journey to Sens-AI** — See what AI can do, where it goes wrong, and why we need a framework that teaches developers better habits.

2. **Setting the AI Up to Succeed** — Learn how to give the AI what it needs to be useful, with clear goals, the right context, and your own research.

3. **Becoming a Better Developer** — Practice problem framing, refining, and critical thinking so you can balance fast AI-assisted coding with the careful judgment that good development demands.

## Additional Resources

- [*Head First C#* (5th Edition)](https://learning.oreilly.com/library/view/head-first-c/9781098141783/) — The code samples in this repo are from Chapter 3
- [*Learning GitHub Copilot*](https://learning.oreilly.com/library/view/learning-github-copilot/9781098164645/) by Brent Laster
- [*AI-Assisted Programming*](https://learning.oreilly.com/library/view/ai-assisted-programming/9781098164553/) by Tom Taulli
- [*Beyond Vibe Coding*](https://learning.oreilly.com/library/view/beyond-vibe-coding/9798341634749/) by Addy Osmani
- [*Prompt Engineering for Generative AI*](https://learning.oreilly.com/library/view/prompt-engineering-for/9781098153427/) by James Phoenix & Mike Taylor

## Contact

- LinkedIn: [linkedin.com/in/andrewstellman](https://linkedin.com/in/andrewstellman/)
- GitHub: [github.com/andrewstellman](https://github.com/andrewstellman)
- More links: [linktr.ee/andrewstellman](https://linktr.ee/andrewstellman)

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/920fe6e4-8d5c-482f-a601-4ccacc7f60d6" />
