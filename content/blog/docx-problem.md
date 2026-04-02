---
title: "The Docx Problem — And Why It Won't Be Legaltech's Edge for Long"
date: 2026-04-02
tags: ["AI", "legaltech", "docx"]
---

Harvey recently published [a post on their new docx editing system](https://www.harvey.ai/blog/building-an-agent-for-complex-document-drafting-and-editing). By improving only the system that reads from and writes to the Word file - not the underlying AI - users accepted 40% more edits.

It's the latest chapter in legaltech's long battle with the docx format. AI promises to transform legal work, but it still has to go through the docx file to get there. And the docx format is genuinely hard for AI to work with - the file structure behind a Word document is surprisingly complex. I'm a lawyer who used to work on Microsoft Office, so this is a problem I watch closely.

Right now, legaltech tools like Harvey have a real edge over general-purpose models when it comes to working with Word documents.

My prediction: within a year, the general-purpose tools are going to get a lot better at editing docx files. For the longest and most complex documents, purpose-built solutions may still have an edge. But for most lawyers, the gap will close. Legaltech tools can still differentiate in other ways, but docx handling won't be one of them.

## The docx layer

Here's what the complexity looks like in practice: Even bolding a single word in a word doc changes the underlying file structure in ways that can break other parts of the document. If you're curious about the technical details, Harvey's earlier post has a good walkthrough.

That complexity is why AI has a hard time with Word documents. Upload a contract to Claude, ChatGPT, or Gemini and ask it to make edits. On simple tasks it (mostly) works fine. But as the complexity grows, things break. Formatting gets lost. Tracked changes get corrupted. Edits land in the wrong place.

## Testing the gap

I wanted to test two things: (1) how good is Claude's out-of-the-box experience for editing docx files; and (2) could I approximate Harvey's approach and close the gap?

So I fed Harvey's blog post to Claude Code and built an agent following their core principle: strip the file down to what matters (the text) - give the model tools to make specific edits to a copy of the document in memory, and let it check its own work. It took an afternoon.

Then I ran 50 tests covering simple edits lawyers actually make - simple find-and-replace, editing tables, rebranding a document, conforming an agreement to a term sheet, repurposing a contract for a new jurisdiction, making scattered edits across 150-paragraph documents.

You can see what I tested and the results [here](https://nberk.github.io/llm-docx-editing/showcase/).

![Test results showing 50/50 for the agent approach and 43/50 for Claude's built-in docx skill](/docx-experiment-results.jpg)

Claude's built-in docx handling passed 43 out of 50. It couldn't fill in form field placeholders. It couldn't conform an agreement to a term sheet. It missed edits in long documents, couldn't fully switch a contract's legal posture, and left a typo behind in a proofreading task.

The agent passed all 50.

This isn't a comprehensive benchmark (I had Claude generate the test cases and spot checked the results). But it shows that docx editing has not been a priority for the general-purpose model providers or Microsoft. I was able to make meaningful improvements in an afternoon.

## This is changing quickly

Progress in docx editing is coming from every direction - legaltech vendors, model providers, open-source projects, and individual builders. When a problem is being attacked from many angles, it doesn't stay a differentiator for long.

[Vesence](https://www.vesence.com/), a legaltech startup backed by some famous investors (Y Combinator, Paul Graham), built a proprietary "Word Engine" from scratch last year. As they put it, "AI is great with plain text, but docx files are a nightmare." The product looks genuinely promising, and I expect we'll see others like it. The more startups that invest in solving this problem, the faster the solution becomes a commodity.

SuperDoc just [open-sourced a document engine](https://www.superdoc.dev/changelog/2026-03-22-document-engine%20) for AI agents to edit docx files with full preservation of the underlying structure - the kind of shared infrastructure that turns hard engineering problems into commodities.

Individual developers are making progress too. Communities like [Legal Quants](https://www.legalquants.com/) are building and sharing their own AI-powered document tools - work that used to require dedicated engineering teams.

It's also notable who was late to the game. For years, Microsoft didn't seem to be making much progress. Their [Wave 3 update](https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/powering-frontier-transformation-with-copilot-and-agents/), shipped in March, is a significant investment in AI editing inside Word. And Word is expected to let you choose between OpenAI and Anthropic this month. Microsoft is (finally) making moves.

And Anthropic has released Excel and PowerPoint add-ins...but not Word. This seems like an obvious next step.

## What this means

For most lawyers, this is good news. The docx problem has been a real bottleneck - AI that can reason about legal documents but can't reliably write them back to a Word file isn't very useful.

Legaltech providers will still have plenty of ways to add value - access to firm knowledge, domain-specific workflows, etc. But the docx advantage specifically won't be one of them.
