---
title: "Beyond the Hype"
date: 2025-04-02
tags: ["AI", "law", "legaltech", "benchmarks"]
---

How should I be using AI in my practice? What is it good at? How does it compare to human lawyers?

It's difficult to answer these questions. The technology is evolving rapidly, and every week providers announce new capabilities. It's hard to separate hype from reality.

Fortunately, independent researchers are stepping in to test current tools - and create benchmarks to help evaluate tools moving forward.

**In this post, I'll summarize two recent studies that tested how well AI performs, or helps with, realistic assignments - the kind of work practicing lawyers do every day.**

1. A University of Minnesota study that compared the work product of law students working with AI to the work product of law students working without AI: [AI-Powered Lawyering: AI Reasoning Models, Retrieval Augmented Generation, and the Future of Legal Practice](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5162111).
2. A study from Vals AI (an independent research company that specializes in benchmarking), that compared AI legal tools against human lawyers by having each work separately (not collaboratively) on the exact same set of legal tasks: [The Vals AI Legal Report](https://www.vals.ai/vlair). (They will perform this benchmark annually and are also working on a separate test for legal reasoning).

**After summarizing the studies, I'll share practical takeaways that will empower any lawyer to start using AI.** You'll get a framework for thinking about AI adoption that focuses on incremental wins, rather than wholesale transformation, allowing you to start benefiting from AI immediately without disrupting your practice.

The research suggests that using AI - particularly when combined with human oversight - is already producing work that can exceed what attorneys create working alone. It also suggests AI alone can already perform certain tasks better than humans - in a fraction of the time. However, these tools still make significant errors and require careful review.

## Minnesota Study (Lawyers _with_ AI vs. Lawyers _without_ AI)

### Overview

- **What they tested**: Does AI help lawyers produce better work than lawyers working alone?

- **How they tested it**: 127 law students completed legal assignments that junior associates would do at a law firm. Each student completed six assignments in three ways: two without AI, two with a legal-specific AI tool (Vincent AI) and two with a general-purpose AI tool (OpenAI's o1-preview).

- **AI tools tested**

  - OpenAI's o1-Preview (Non-legal specific)
  - VLex's Vincent AI (legal-specific)

- **Who evaluated the work**: Three experienced lawyers who didn't know which assignments used AI.

- **How they scored it**: Five categories, each on a scale of 1-7
  - _Accuracy_: Precision and usefulness of research
  - _Analysis_: Depth and insightfulness
  - _Organization_: Clarity and structure of work
  - _Clarity_: Quality and persuasiveness of writing
  - _Professionalism_: How well directions were followed
  - They also counted mistakes ("hallucinations")

### Tasks

- **Draft Client Email** - Draft a concise, research-backed email (under 700 words) explaining to a client why a defamation claim cannot be based on statements made solely within litigation. Students had to reference authoritative case law or statutes within the Tenth Circuit jurisdiction. Time limit: 60 minutes.

- **Draft Legal Memo** - Create an objective legal research memo (under 1,500 words) analyzing whether, under Massachusetts and New Hampshire insurance laws, an insurer must pay $200,000 in attorneys' fees in addition to a $2 million liability coverage limit. Students were provided with the relevant insurance policy language and instructed to consider case law while distinguishing applicable precedents. Time limit: 240 minutes.

- **Analyze Complaint** - Draft a concise memo (under 1,000 words) summarizing key allegations and claims in a class action complaint, assessing the strength of these claims, and outlining potential defense strategies. Students were provided with the complaint from a real federal court case. Time limit: 120 minutes.

- **Draft NDA** - Create a concise, enforceable non-disclosure agreement that protects a company's proprietary trade secrets while complying with legal limitations in Minnesota and neighboring states. The NDA needed to be written in plain English, favorable to the company, and no more than three single-spaced pages. Students were provided with an overbroad sample NDA as a starting point. Time limit: 180 minutes.

- **Draft Motion to Consolidate** - Prepare a persuasive brief (under 1,000 words) supporting a motion to consolidate two cases in Minnesota state court that share overlapping facts and issues. Students had to advocate for consolidation to ensure efficiency and consistency while citing Minnesota case law and civil procedure rules. Time limit: 150 minutes.

- **Draft Persuasive Letter** - Write a persuasive letter (under 1,250 words) arguing that a covenant not to compete signed by a restaurant's former chef is reasonable and enforceable under Indiana law. Students needed to demonstrate that the scope, geographic restrictions, and duration of the covenant are justified to protect the restaurant's legitimate business interests. Time limit: 150 minutes.

### Results

Legend:

- ✅ = AI + Human beat human lawyers (% quality improvement vs. no AI assistance)
- ❌ = AI + Human _did not_ beat human lawyers

|         Assignment          | o1-preview (general-purpose AI tool) <br/> + Human | Vincent AI (legal-specific AI tool) + Human |
| :-------------------------: | :------------------------------------------------: | :-----------------------------------------: |
|      Draft Legal Memo       |                     ✅ +23.6%                      |                  ✅ +13.5%                  |
|      Analyze Complaint      |                     ✅ +10.2%                      |                  ✅ +8.0%                   |
| Draft Motion to Consolidate |                     ✅ +28.1%                      |                  ✅ +12.0%                  |
|     Draft Client Email      |                      ✅ +9.5%                      |                  ✅ +15.1%                  |
|   Draft Persuasive Letter   |                     ✅ +20.9%                      |                  ❌ -8.9%                   |
|          Draft NDA          |                      ❌ -4.2%                      |         ❌ +0.3% (not significant)          |

## Vals AI Study (AI Tools vs. Human Lawyers)

### Overview

- **What they tested**: How do AI tools perform compared to human lawyers?

- **How they tested it**: They created a benchmark of 200+ tasks, grouped into seven categories. Human lawyers completed all tasks (regular practicing lawyers who thought they were doing actual client work). The AI companies were allowed to decide in which task categories their tools were scored.

- **AI tools they tested**:
  - CoCounsel (from Thomson Reuters)
  - Vincent AI (from vLex)
  - Harvey Assistant (from Harvey)
  - Oliver (from Vecflow)
- **How they scored it**: They created a checklist of what a correct answer should include, then used an automated system to check if each answer included those elements.

### Tasks

| **Category (# Qs)**                                             | **What It Tests**                                                                                                                                                                                                                                                                                                                                                                                                                                                       | **Example Question**                                                                                                                                                                                                                                                                                                       |
| --------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Data Extraction** (30 questions)                              | The ability to identify and extract specific information from documents                                                                                                                                                                                                                                                                                                                                                                                                 | "Extract the exact text of the assignment clause from this agreement."                                                                                                                                                                                                                                                     |
| **Document Q&A** (30 questions)                                 | The ability to review and analyze information in a document to answer specific questions                                                                                                                                                                                                                                                                                                                                                                                | "What do I do if an employee says they can't work on certain weekdays for religious reasons?"(Asked with document called “Religious Discrimination Guidance”, a 167 page document from the US Equal Employment Opportunity Commission)                                                                                     |
| **Document Summarization** (20 questions with unique documents) | The ability to accurately and fully summarize a whole document or specific parts of a document                                                                                                                                                                                                                                                                                                                                                                          | "Provide a one paragraph summary of the new filing requirements under the final rule."(Document provided: FinCen's AML requirement, a 100 page document with three-column layout, tables, and figures)                                                                                                                     |
| **Redlining** (20 questions)                                    | Capabilities relevant to the review and negotiation of a contract by doing one of three things: (1) suggesting an amendment to a provision or contract to bring it in line with a provided standard; (2) identify whether certain terms match a provided standard and, if not, suggest an amendment to bring it in line; and (3) review a redlined contract, identify the changes and explain the impact of the changes and/or recommended steps to address the changes | "What changes have been made to the license agreement and what is the impact of those changes?"                                                                                                                                                                                                                            |
| **Transcript Analysis** (30 questions)                          | The ability to review and analyze information in court transcripts                                                                                                                                                                                                                                                                                                                                                                                                      | "How many lawyers were present to represent Elizabeth?" (Reference document: Holmes Transcript July 11, 2017)                                                                                                                                                                                                              |
| **Chronology Generation** (10 questions)                        | The ability to identify, describe, and order specified events or facts from a document                                                                                                                                                                                                                                                                                                                                                                                  | "Generate a chronology of the underlying facts of this case and the procedural milestones of the NLRB in reaching its decision (including the date the decision was delivered). The output should consist of a list setting out each key date (month, day and year) with a concise summary of what happened on that date.” |
| **EDGAR Research** (100 questions)                              | The ability to assist in broad market-based research or answer specific questions relating to U.S. public companies by reference to the SEC's EDGAR database.                                                                                                                                                                                                                                                                                                           | "When is the last day that shareholders of the BlackRock Future Tech ETF were able to sell their holdings on NYSE Arca?"                                                                                                                                                                                                   |

### Results

Legend:

- ✅ = AI tool beat human lawyers
- ❌ = Participated but didn't beat lawyers
- ⚪ = AI tool did not participate

|       **Legal Task**       | **CoCounsel** | **Vincent AI** | **Harvey Assistant** | **Oliver** |   **Task Winner**    |
| :------------------------: | :-----------: | :------------: | :------------------: | :--------: | :------------------: |
|    **Data Extraction**     |      ✅       |       ❌       |          ✅          |     ❌     |        Harvey        |
|      **Document Q&A**      |      ✅       |       ❌       |          ✅          |     ✅     |        Harvey        |
| **Document Summarization** |      ✅       |       ✅       |          ✅          |     ✅     |      CoCounsel       |
|       **Redlining**        |      ⚪       |       ❌       |          ❌          |     ⚪     |       Lawyers        |
|  **Transcript Analysis**   |      ⚪       |       ✅       |          ✅          |     ⚪     |        Harvey        |
| **Chronology Generation**  |      ❌       |       ⚪       |          ✅          |     ❌     | Harvey/Lawyers (tie) |
|     **EDGAR Research**     |      ⚪       |       ⚪       |          ⚪          |     ❌     |       Lawyers        |

## Takeaways

Given how quickly the technology is changing, I won't comment on the performance of particular tools (many of the tools tested have new versions). These results are very much a (now slightly outdated) snapshot of how well these tools perform.

The studies have a detailed analysis of the nuances of how tools performed; I highly recommend reading.

### General Advice for Approaching AI

#### Think in Tasks, Not Entire Assignments

The most successful approach to using legal AI isn't asking “Can AI handle a complete assignment?” but rather “which specific tasks within my workflow could AI assist with?”

The Vals AI study provides a useful set of categories of tasks that AI can assist with. These tasks are generally part of a bigger assignment (rarely does a client ask you to summarize a document).

Over time, AI tools will evolve to handle more, and more complicated, workflows (_e.g._, drafting an entire complaint, drafting a complete S-4). But, given the current capabilities, it's best to think about the individual tasks.

#### Conduct Small Scale Experiments

The best way to understand AI's capabilities for your practice is through experimentation:

1. Select a recently completed matter
2. Identify 2-3 discrete tasks from that matter
3. Run these tasks through AI tools
4. Compare AI output with your original work product

#### Create Your Own Benchmarks

As your firm experiments with AI, systematically build your own "benchmark library" to track progress over time.

Keep track of the type of tasks that you try AI for - and track the successes and failures. Revisit tasks that failed as new tools get released.

This approach helps track AI capabilities specific to your practice area, helping you make informed decisions about which tasks to delegate to AI and which still require primarily human attention.

#### Compare AI to Real Lawyers, not Perfect Ones

These studies highlight that human lawyers make mistakes, too. This is particularly true for time-consuming tasks that require a lot of concentration, like reviewing, or searching for questions in, long documents.

When evaluating AI output, remember:

- The standard isn't perfection but rather what a human lawyer would produce
- Human lawyers sometimes cite cases incorrectly or miss arguments (the data in the studies supports this).
- The speed advantage of AI may outweigh minor quality differences for some tasks.

### Practical Advice Based on Tools' Current Capabilities

#### Start with Document-Focused Tasks

Both studies indicate AI currently performs particularly well when working with existing documents, such as:

- Summarizing contracts or pleadings
- Extracting key information from long documents
- Answering specific questions about document content
- Analyzing complaints

The Vals AI Study specifically noted that: "Document Q&A produced the highest scores out of any task in the study, and is a task that lawyers should find value in using generative AI for."

For example (although it's not strictly legal) - I used AI extensively to write this post, by uploading the studies and asking questions about them. And, while it made mistakes and I had to verify the facts, it generally did a great job! And it was a great brainstorming partner.

#### Leverage AI to Improve Writing Quality, Even When You Don't Trust the Analysis

Even when you don't trust AI for substantive legal analysis, it can still improve your writing. Consider pasting your work into an AI tool after you've finished a draft and asking it to:

- Edit for clarity and conciseness
- Convert complex legal concepts into plain language for clients
- Identify grammatical issues and typos
- Reorganize information for better flow

As the Minnesota researchers noted, AI-assisted work was "easier to read and more polished" with "more concise" sentences and "smoother" paragraph flow.

#### Leverage AI for Speed: Create First Drafts in Minutes, Not Hours

Both studies highlighted the dramatic speed improvements that AI tools produced. In the Minnesota study, AI reduced completion times by 14-37% across most tasks.

Instead of spending hours creating a basic first draft, focus your expertise on editing, fact-checking, customizing, and adding strategic value to work product.

#### Always Verify: AI Makes Significant Mistakes

While AI shows impressive capabilities, both studies emphasized that these tools still make significant errors. Key verification steps include:

- Cross-check every legal citation to confirm it exists and says what AI claims
- Verify all factual assertions against source materials
- Review reasoning for logical gaps or unsupported conclusions

## Reference - List of AI Tools Tested

- CoCounsel (from Thomson Reuters): [CoCounsel: One GenAI assistant for professionals | Thomson Reuters](https://www.thomsonreuters.com/en/cocounsel)
- Vincent AI (from vLex): [vLex | Vincent AI](https://vlex.com/vincent-ai)
- Harvey Assistant (Harvey): [Harvey AI](https://www.harvey.ai/)
- Oliver (Vecflow): [Vecflow](https://www.vecflow.ai/)
- OpenAI's reasoning model: [OpenAI](https://openai.com/) (not legal-specific)
