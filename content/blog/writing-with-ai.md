---
title: "Good Writing is Good Thinking. AI Can Help."
date: 2026-03-22
tags: ["writing", "AI", "creativity"]
---

My dad taught me to love good writing. His favorite quote is "I'm sorry I wrote such a long letter; I didn't have time to write a short one." I can still picture the red ink all over my grade school papers. He edited my writing ruthlessly, for as long as I can remember. I understood from an early age that writing is not just about the words on the page - it's about all the thinking that comes before. It's about respecting the reader and their time.

<p style="text-align:center">* * *</p>

Right now, it feels taboo to use AI to write. When people think about using AI for writing, they assume the result is going to be AI slop - thoughtless, generic. It's seen primarily as a time saver - an attempt to outsource thought and automate the writing process. It's fine for simple writing - emails, straightforward blog posts. But it shouldn't be used for writing that "matters."

In this post, I explain how AI, used well, produces *better* writing. I show how it doesn't *replace* my thinking, it sharpens it. I share my workflow, including example [prompts](#prompts-i-use).

<p style="text-align:center">* * *</p>

Good writing is good thinking. The words on the page are the *output* of clear thinking. When people say they're "struggling to write" they don't mean they can't construct sentences, they mean they don't know what they want to say.

And it's very rare to sit down to write knowing exactly what you want to say. In Anne Lamott's famous essay, "[Shitty first drafts](https://wrd.as.uky.edu/sites/default/files/1-Shitty%20First%20Drafts.pdf)," she argues that all good writing starts as a mess. Nobody produces polished prose on the first try. The first draft is about getting the chaos out of your head so you can find the good stuff buried in it.

AI accelerates the process of finding the good stuff. When I'm in the mess, it lets me experiment. When I have something but I'm not sure it's right, it acts like a critical colleague: pushing back on the argument, suggesting alternatives. And when I know something is wrong but can't pinpoint why, it proposes fixes.

The key is to see AI as a tool you *collaborate with* to write - not as a tool that produces writing.

*On scope for this piece: I'm focused on functional writing - explanatory and persuasive prose. Some of this will apply to more "creative" writing - but that has a different set of considerations*.

## How I write with AI

Here's what that looks like in practice.

### Start with a brain dump

Before I open AI, I dump all my thoughts about the topic into a document. All of it - messy, contradictory, half-formed. I don't edit. I just get the ideas out of my head. This is the terrible first draft. **It's critical to have a foundation that's *mine* before AI enters the picture**. AI is great at organizing and refining ideas. It is not great at generating the underlying conviction.

### Hand the mess to AI

Once I have the brain dump, I open Claude. I create a Project (Claude's system for organizing related chats and other resources)for the piece, and upload the brain dump along with any reference material - source documents, research. Then I ask Claude to find the themes and patterns.

For this post, for example, I started with a sprawl of notes about how I use AI to write, with half-formed points about experimentation, structure, discipline. I uploaded it and said: "*I'm writing a post about how to use LLMs in the writing process. Here is a brain dump of thoughts. I want to focus on the framing of the iteration between figuring out what you want to say and figuring out the best way to say it.*" (I usually include some guidance with the brain dump about what I *think* I want to focus on - but that often changes.)

Claude came back with a proposed structure - themes it found in my notes in a logical order, a suggestion for how to frame the argument. Some of it worked. Some of it didn't. I go back and forth with Claude to clarify what I want to focus on.

From that initial structure, I have Claude write a full first draft. It's usually bad, but that's okay. Seeing what doesn't work moves things forward by giving me something to react to. This is an "AI-assisted shitty first draft."

### The back-and-forth

From here, the process splits into two tracks: a Google Doc and a Claude chat.

AI never touches the Google Doc - that's what keeps me in control.

I start both fresh. I open a new Google Doc and a new Claude chat, and give Claude the most recent draft (initially, that's the draft from the brainstorming phase). Then I edit collaboratively in Claude: changing arguments, moving things around, trying different openings, cutting. (See below for specific prompts and advice).

When a section is good enough, I type it into the Google Doc myself, often making additional changes at that point.

By the end of a round, the Google Doc has moved ahead of what Claude has seen. So I reset - new Google Doc, new Claude chat. I paste the updated draft from Google Docs into Claude and go again. I usually go through two to four full rounds.

![My writing setup: Google Doc on the left, Claude on the right](/writing-with-ai-setup.png)

### This post as an example

This post went through several rounds. In the first, the structure wasn't working; the piece had a clear organizing principle on paper, but when I read the full draft it didn't feel right.

So I opened a new chat and said: "It is really a mess. I do not like the structure. I have a lot of things that I want to say, and I think they're getting jumbled. Help me disentangle." Claude diagnosed the problem: I was threading three things through the piece at once: the philosophy, the process, and a bunch of tips. They were bleeding into each other.

Then Claude asked clarifying questions. *What's the central argument? Who's the audience? What should the reader walk away with?* I discovered I wanted the piece to be primarily practical. With that framing, we experimented with a few ideas - and, from that, a new structure emerged: lay the philosophical foundation first, then walk through the practical process. That's the structure you're reading now.

None of that was in my original notes. AI didn't figure it out for me. It gave me material to analyze, and my reactions told me what I actually thought.

## Polish

As the draft gets closer to done, the work shifts. I'm no longer restructuring or rethinking the big ideas, I'm cleaning. I use AI for this too: asking it to find redundant ideas, cut unnecessary words and filler, flag clunky phrases. It's good at this - faster and more systematic than I am.

I do the final pass alone. I go through the whole thing without AI, making sure it makes sense, catching anything that got smoothed over but isn't quite right.

## Tips

Here are some specific things I've learned working with AI to write.

**Focus on the big picture first.** What's the argument? What's the structure? What goes where? I don't worry about awkward sentences or rough transitions initially (though sometimes I can't resist editing them early).

**Ask AI what it thinks you're trying to say**. The prompt *What would you say my main argument is in this piece?* is one of the most useful prompts I've found. It helps me clarify my own thoughts, and it also helps me direct AI to the right understanding.

**Use outlines to see structural problems**. Ask AI to outline what you've written *What are the main points, and what's the progression*? Then, you can review the result, and even ask AI to do the same ("*does that progression make sense? Is there an opportunity to clarify?"*).

I used this in the introduction to this post. I had five paragraphs making variations of the same argument, and the outline made it visible immediately. I compressed it to three. I often can't see structural problems from inside the prose; the outline surfaces them.

**Pay attention to AI's assumptions**. AI forms its own interpretation of what you're writing, and sometimes that interpretation has a key assumption wrong. It's like talking to a smart colleague who's missing a key premise. I can tell something isn't landing, but I can't pinpoint why - until I realize the AI thinks I'm arguing X when I'm really arguing Y. Correct it, and the conversation clicks.

For example, in this piece, Claude initially assumed the post was about what people do *wrong* with AI. It thought I was trying to chide people for not thinking (AI seems to default to being snarky and glib for persuasive posts) so it kept framing things around "the problem with skipping the hard part." But I wasn't trying to *correct* people, I was trying to explain how to use AI effectively. Once I corrected that assumption, the suggestions got sharper.

**Keep track of how edits ripple through the piece.** When AI makes a change in one place, it can create clunky transitions or contradictions elsewhere, and it won't always notice. You can ask Claude to review how a change affects other sections, and it'll often catch things. But ultimately you're the one who has to hold the whole piece in your head and make sure it still works.

**Close the AI window**. Periodically, I stop using AI. I go back to just the document. It's easy to fall into a pattern of cycling through AI outputs without stopping to ask: *do I actually agree with this?* I go back to staring at the page and thinking *what do I really want to say here*? Sometimes the answer is different from what the AI and I had been building toward.

**Delete aggressively**. No matter how much I prompt AI to be concise, to remove duplication, to cut unnecessary words, it's wordy. AI-produced text almost always needs to be shorter. Cut aggressively. This is one of the most important things humans bring to the process: the willingness to kill sentences that technically work but aren't earning their place.

**Build a writing instruction set.** After working with AI for a while, I asked it to review my past interactions and create a custom style guide: *Review our recent conversations about writing. Identify patterns in my voice, structure preferences, and the edits I make repeatedly. Build a custom instruction set that another conversation could use to match my style.*

## Prompts I use

### Getting started

- *Here's a brain dump of thoughts on topic. I want to focus on specific framing. Help me find a structure.*
- *I have a lot of things I want to say and they're getting jumbled. Help me disentangle.*
- *Let's have a back and forth where you ask me clarifying questions to make sure the point is here.*

### Working on the argument

- *What would you say my main argument is in this piece?*
- *I want to include this idea - but I'm not sure about it. Push back on me.*
- *I want to say something like messy version of a point. Help me make that clearer.*
- *Outline this section. What are the main points, and what's the progression?*

### Restructuring

- *I don't like the structure. Here's what I think the problem is: diagnosis. How should we reorganize?*
- *What if I lead with X instead of Y?*
- *I want to make this new point. Where in the piece should it go?*

### Fixing specific problems

- *This paragraph doesn't make sense. Here's what I'm actually trying to say [messy version]. Clean that up.*
- *There are repetitive elements. Go through the piece, identify the points, and reduce duplication.*
- *This section feels off, but I can't pinpoint why.*

## Conclusion

Orwell said "good prose is like a windowpane." The writing disappears - you see straight through to the idea. That's what good writing has always been.

AI just changes how much help you have getting there. The back-and-forth, the experimentation, the ability to try ten approaches and find the one that works - the writing is better for it.

If you have something you want to say - an idea that's been rattling around in your head, an argument you haven't quite figured out - it's never been easier, or more fun, to express it clearly.
