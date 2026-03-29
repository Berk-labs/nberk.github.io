---
title: "How to Actually Learn with (or without) AI"
date: 2026-03-29
tags: ["learning", "AI", "education"]
---

This may sound familiar: you want to learn about something, so you ask AI to teach you. A perfectly clear explanation streams back - well-structured, tailored to your level, easy to follow. A warm sense of understanding washes over you. You feel smarter.

That feeling is mostly a lie. (gasp!)

Not every interaction needs to be deep learning - sometimes you just want a quick answer or the gist of something, and that's fine. But if you're trying to *really* learn something - how to read a financial statement, what started World War I, how interest rates work - it's worth knowing what actually makes learning stick.

I want to save you time, and help you learn more. I was a good student in part because of crippling anxiety and a deep fear of failure, but also because I love learning. And there are a few basics that make it easier to learn *anything*, whether you're using AI or not.

**I'll tell you up front: the single simplest change you can make is to ask AI to teach you by asking you questions and quizzing you. If you really want to learn it, open that conversation over the following weeks and test your understanding again** (I built an open source app around this idea - more on this later).

## Desirable Difficulties

When something is easy to read, our brains assume we understand it. Psychologists call this an **"illusion of competence."**[^1] Your brain confuses recognition - seeing it and thinking "that makes sense" - with recall, which is what you'll actually need later.

AI makes this illusion worse because its explanations are so clear and polished. You read Claude's explanation of monetary policy and think "got it." An hour later, you couldn't explain it to anyone.

For learning to stick, your brain has to do work. Psychologists call the conditions that create this work **"desirable difficulties."**[^2] Reaching for an answer, getting something wrong, sitting with that uncomfortable blankness - that's what builds memory. It doesn't have to feel *painful* - it can be absorbing, even fun. But if it feels completely effortless, you're probably not learning.

Reading generally doesn't create desirable difficulty. Neither does rereading, highlighting, or reviewing your notes. Those feel productive, but you're not making your brain work - you're just spending time with the material. It's like going to the gym and just walking around. You go home and can honestly say you "went to the gym." But nothing happened.

One way to create desirable difficulty is to force yourself to recall the information. Psychologists call this **retrieval practice**, and the finding behind it is one of the most replicated in learning science: being quizzed on material produces stronger memory than rereading it, even when the quiz happens right after you learn something.[^3]

## Using AI to Learn

AI makes retrieval practice simple. Tell it to teach you by asking questions and to demand precise answers. That's it.

It works even when you're starting from zero. AI doesn't open with something you couldn't possibly answer - it finds where you are and builds up.

Say you want to learn how planes fly. It doesn't start with "describe Bernoulli's principle." It asks "What do you think is actually holding a plane up in the air?" You have some intuition - something about the wings, maybe air pushing underneath. You say so. It pushes: "Okay, so what's different about the top of the wing versus the bottom?" Now you're reasoning your way toward lift instead of reading a textbook definition.

You'll find this works surprisingly well. You don't need fancy prompts. But if you do this often and want to stop repeating yourself, you can save prompts that set up the interaction. I added a [/tutor command](https://github.com/nberk/claude-code-setup/blob/main/commands/tutor.md) to my Claude Code setup that teaches by asking questions instead of explaining, and a [/quiz command](https://github.com/nberk/claude-code-setup/blob/main/commands/quiz.md) for when I'm coding and I want to understand the changes we made.

I also look for opportunities to go beyond simple Q&A. For example, when I wanted to learn Chrome's web dev tools, I asked for an [interactive lesson](https://github.com/nberk/web-dev-tools-exploration) where I had to use the tools to find answers myself.

## Codifying It: Building Socratic

The quiz approach got me most of the way. But retrieval practice has a gap: memory still fades over time. It's not just *whether* you review - *when* you review matters too.[^4] Memory decays on a predictable curve - most of it within the first day or two. But if you recall something right as it's about to fade, the memory resets and lasts longer than before. Do it again at the right moment, and the interval stretches further. (Anki is the most famous version of this - IYKYK.)

Timing those reviews by hand is hard. So I built [Socratic](https://socratic-learning.fly.dev/) - a simple, [open source](https://github.com/nberk/socratic) app that pulls all of this together (the name is a nod to the Socratic method - Socrates taught by asking his students questions rather than giving them answers). It creates a lesson plan, quizzes you section-by-section, then schedules reviews over the coming days and weeks. Demonstrate understanding and it waits longer before the next review. Get something wrong and it comes back sooner.

It takes work — but the moment I can explain something I couldn't before makes it worth it.

![Socratic app welcome screen for an Introduction to Quantum Physics lesson](/socratic-dashboard.png)

[^1]: [Koriat & Bjork, "Illusions of Competence in Monitoring One's Knowledge During Study"](https://doi.org/10.1037/0278-7393.31.2.187) (2005). Demonstrated that learners' predictions of their own recall are driven by perceived relatedness during study rather than actual retrievability at test.

[^2]: [Bjork, "Memory and Metamemory Considerations in the Training of Human Beings"](https://bjorklab.psych.ucla.edu/wp-content/uploads/sites/13/2016/04/RBjork_1994.pdf) (1994). Introduced the concept of "desirable difficulties" — conditions that make learning harder in the short term but more durable in the long term. Besides retrieval practice, other desirable difficulties include: spacing (distributing practice over time instead of cramming), interleaving (mixing different topics or problem types during practice), generation (producing an answer yourself before being shown it, even if you get it wrong), and variation (changing the conditions of practice so knowledge transfers more flexibly).

[^3]: [Roediger & Karpicke, "Test-Enhanced Learning: Taking Memory Tests Improves Long-Term Retention"](https://doi.org/10.1111/j.1467-9280.2006.01693.x) (2006). Students who took a practice test after reading a passage retained significantly more than students who reread it — even though the rereaders felt more confident. A [meta-analysis by Rowland](https://doi.org/10.1037/a0037559) (2014) of 159 comparisons confirmed a significant testing effect, with the advantage of retrieval practice being larger on delayed tests than immediate ones.

[^4]: The foundational research here is [Ebbinghaus, *Memory: A Contribution to Experimental Psychology*](https://psychclassics.yorku.ca/Ebbinghaus/index.htm) (1885), who discovered that memory decays rapidly after learning but that each successful recall flattens the curve — the interval before you'd forget again gets longer each time. [Cepeda et al., "Distributed Practice in Verbal Recall Tasks"](https://doi.org/10.1037/0033-2909.132.3.354) (2006) confirmed this with a meta-analysis of hundreds of studies: spacing practice over time reliably improves retention, and the optimal gap between reviews is roughly 10-20% of the time until you'll need the information.
