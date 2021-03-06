+++
title = "Tutorial guidelines"
description = "Our guidelines to write guides and tutorials that serve our users as well as we can."
author = "nathan"

date = 2021-01-03
weight = 5
+++

In this guide, you'll find our guidelines to write guides and tutorials that serve our users as well as we can. We'll also present our recommended writing workflow and tools you should use to help simplify your writing.

Our goal is to help students follow along and learn as much as possible from our content. We always strive to **help others**, **empathize** with them, and **lower the cognitive load** involved in learning something as complicated as game development.

To achieve this goal, **clarity**, writing plainly and explicitly, is critical.

To achieve this, you want to:

1. **Put yourself in the reader's shoes**. Start where they are, avoiding unnecessary jargon and complexity.
1. **Focus on one thing at a time**, be it a new concept, problem, technique, or set of instructions.
1. **Structure** your content to make it as easy as possible to follow.
1. Always explain "why", more so than "how".
1. **Seek critical feedback** from teammates and target users and use it to improve your content.

We can use more concrete style guidelines to put the principles above into practice:

1. Explain what the reader will learn and what the prerequisites are at the start.
2. Start from the users' problems.
3. Use **concrete examples** that are relevant to the problem at hand.
4. Favor explicit language; avoid long and indirect sentences.
5. Favor common words over literary terms. Always remember we write for both native and non-native speakers.
6. **Repeat keywords** to reinforce the reader's understanding of new concepts.
7. Keep images simple and as close as possible to the relevant text.
8. Use consistent formatting rules. _Italics_ when referring to labels in the user interface, `inline code` for any reference to a symbol, expression, or value, and **bold** to **emphasize** an important concept, keyword, or takeaway.

## Put yourself in the reader's shoes

**Start where the reader is**. Help them solve _their_ problems, write with the vocabulary _they_ have.

To do so, try to remember how it was when _you_ were learning this concept for the first time. What was it you struggled with the most? Which terms or ideas did you not understand?

Ensure that you explain those terms and concepts to the reader or provide them with the necessary resources to learn.

## Focus on one thing at a time

The reader is learning from you, meaning they have to take in new information. The easiest way to do so is to deliver one bit at a time and repeat terms or ideas and link them to new ones progressively.

Covering one concept at a time is a principle you should apply at different levels in your writings.

For example, within a series, each lesson should focus on a given problem, theme, or technique. You want to avoid bloating a lesson with irrelevant content. If necessary, you can split the topic into two.

Inside a tutorial, each section should focus on a specific problem described by their **heading**. For example, "animating a sword swing," "understanding the different kinds of noise," or "implementing an inventory."

## Structure your content

Start by explaining what the reader will get out of your guide and what the prerequisites are. Use this to remind yourself of your teaching goals: you are making a promise to the reader, and your tutorial should fulfill it.

Explain the problem or set of issues that you will address. Also, give the user the background or context they need to follow along. This not only helps the reader see the value they can get in reading to the end; it also tells them instantly if this is the content they were looking for, saving them precious time if not. 

Give a brief overview of how you will solve the problems and why you picked that approach over others. You can use a bullet list, pseudocode, a picture (diagram, illustration), a video clip, whichever is most straightforward for the user.

Break down the lesson into sections, each with a descriptive heading that presents a specific problem. For example, write `Snapping to the center of grid cells` instead of `The Grid`, or `Using signals to decouple objects` over `Signals`. Reorder the sections to provide the reader with the most natural or accessible learning flow.

{{< note >}}Writing good headings goes a long way to helping you frame what you will write and stick to it. Always keep the problem at hand and your heading in mind while writing.{{< /note >}}

Finish with a short recap that emphasizes the key takeaways and provides further resources. This helps the reader get a sense of what's most important to memorize. Hint at what the next part will cover if you are writing a series, to motivate them to keep reading.

## Always explain "why"

You always want your content to explain or at least hint at:

1. Why you chose a solution or an approach over another.
1. Why the problem you are trying to solve or the technique you are teaching matters to the reader.

There is more that users consider part of the answer to "why." Some users will feel like you did not answer that question if your guide does not explain the context or the background for the problem at hand well. Or if you didn't read their mind and answer questions that could arise from your guide.

To address that, once again, you need to try to understand the readers' psychology, their situation, and anticipate the questions they might have.

This comes with experience, practice, and the following principle, seeking critical feedback from your target audience.

## Seek critical feedback

Always put the content in the hands of your teammates and users.

It does not matter if you think a lesson is clear if it is not clear to your students.

If a student in the target audience does not understand something, do not blame them or assume anything about them. Do your best to understand the source of confusion and the actions you can take to clarify and improve the content.

The best way to achieve that goal is to ask them questions, especially if they did not provide enough information in their feedback or request.

When giving feedback to a teammate, play the role of a student and ask questions whenever something is unclear, is not covered, or lacks details. This is a great way to guide the writer into fleshing out their content.

## Style

Below are more concrete writing guidelines, with examples.

**Work-in-progress.**

<!-- TODO: add missing guidelines and remove. -->

### Repeat keywords

Repeat keywords. Avoid using synonyms for important terms, labels, and code, as it makes it harder to link elements together.

Avoid varying technical terms for style:

> Godot has a feature to send data without coupling two objects: _signals_. [...] _Send_ a _message_ to have the other node react to the change. [...] Notify the child node with `update_finished`.

Favor repeating the terms and verbs to help the user follow along:

> Godot has a feature to send data without coupling two objects: _signals_. [...] _Emit_ a _signal_ to have the other node react to the change. [...] Notify the child node by _emitting_ the `update_finished` _signal_.

<!-- ### Using pictures -->

<!-- Use many pictures. -->

<!-- Images should illustrate or show the result of an action. -->

<!-- Images should be as close as possible to the relevant text or instruction. Avoid grouping multiple instructions followed by a picture that illustrates a single of them. -->

## The workflow

To write efficiently, **a professional works in three stages**:

1. Outlining.
1. Writing.
1. Editing.

{{< note >}}Before getting to those, you should have your code or demo ready for the tutorial. And, of course, you should have gotten peer-review on the final product.{{< /note >}}

The outline allows you to build a skeleton of the article you're going to write, write down the teaching goals, problems you solve for the user, and headings. It should be easy to spot organization issues at this stage and reorder the headings to provide the best flow possible to the user.

Then comes writing, where you write the content from start to finish without continually stopping to modify or tweak your sentences. The outline gives you the foundations you need to be able to write the content sequentially and productively.

Finally, you want to edit your text. You have to reread it from start to finish and do your best to simplify the writing, clarify the content, but also, if you're making the tutorial, you should follow all the steps and ensure that they lead to the expected result.

Be diligent when you check and refine your writing. If you don't do it carefully, you'll have to return to it and end up with more work later.

You don't have to iterate over it; you then want to send your work to a peer reviewer who will do a second editing pass.

## Tools to use

Use tools to check your writing.

Use a prose linter like [writegood](https://github.com/btford/write-good) to highlight the use of the passive voice, adverbs, and other unnecessarily complicated terms. You should also use a spell checker. 

You don't need to _ always_ check and make corrections as you type. Instead, I would recommend running the tools _after_ you finished writing and using them only during the editing phase.

You should also run your text through an online tool like the [Hemingway app](http://www.hemingwayapp.com/) or [Grammarly](https://grammarly.com) (if you have a premium account) to get more insights regarding sentence length and style.
