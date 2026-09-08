# Chapter 1: What AI actually is

Draft 2 for Mark's review. Pitched at Year 9: technical terms used and explained, no talking down. Mark's own wording used for the opening. Layout notes in [brackets] are for the design pass, not for print.

[Chapter icon suggestion: a speech bubble made of jigsaw pieces. Chapter colour: TBC in design system.]

---

**Standfirst:** Before you use AI, it helps to understand how it works. The real version, not the marketing version.

Here's a question. When you type a prompt into an AI chatbot and it replies in fluent, confident sentences, what's actually happening?

Most people think it works like a database. That it's searching, finding information and then bringing correct answers back to you from verified and correct sources. That simply isn't true, and you'll perhaps be astounded to discover what's really going on behind the scenes.

## It's a prediction machine

You already know more about how AI works than you might think, because you use a small version of it every day. Predictive text. You type "see you" and your phone offers "later", "soon", "tomorrow". It isn't looking those words up anywhere. It has learned, from a huge amount of text, which words tend to follow which, and it gives you its best guess.

That is the core mechanic of every AI chatbot you've used. The difference is scale.

The chatbots themselves are built on what's called a large language model, or LLM, and the name tells you what the thing really is. Large: trained on a colossal quantity of human writing, more than any person could read in thousands of lifetimes. Language: it's about language, not knowledge. Model: a mathematical system that has learned the statistical patterns in all that text. Which words tend to follow which. In what order. In which contexts.

Notice what's missing from that description. Nowhere in an LLM is there a database of verified facts. During training, the model wasn't memorising information and filing it for later. It was tuning billions of internal settings until it became extraordinarily good at one job: predicting the next word. Your keyboard's trick, scaled up so far that the predictions come out as whole fluent paragraphs rather than one word at a time.

So when you send a prompt, the model doesn't go looking for the answer. It generates a response, one word at a time, each word selected because it's statistically probable given your prompt and everything it has produced so far. Run that prediction loop a few hundred times and you get the polished reply on your screen.

[Diagram, full width: "The prediction loop". A sentence mid-generation: "Rain forms when water vapour in the air..." with candidate next words and probability bars: "cools" (long), "rises" (medium), "condenses" (medium), "dances" (near zero). Caption: Every word is a probability calculation. At no point does anything check whether the sentence is true.]

## Probable is not the same as true

This is the single most important idea in this guide, so let's be precise about it.

An LLM is optimised to produce plausible text: writing that fits the pattern of a good answer. Most of the time, the most probable words and the correct words are the same, which is why these tools are right as often as they are. But there is no fact-checking step. The model has no mechanism for telling truth from fiction, because it was never built to. It deals in probability, not accuracy.

That's why an LLM will state something completely false with exactly the same fluency and confidence as something completely true. The confident tone isn't evidence of anything. It's a property of the writing the model learned from: millions of humans who wrote as if they were sure.

Chapter 2 is entirely about what happens when the probabilities go wrong, and what you can do about it.

## It learned from us

One more consequence of how these models are built, and it's a big one.

The training data is human writing. That means the model absorbed our best work: rigorous explanations, careful arguments, brilliant prose. It also absorbed our assumptions, our blind spots and our prejudices, because those run through human writing too, often invisibly.

An LLM doesn't decide to be biased any more than it decides to be wrong. It reflects the patterns in what it was trained on, including the ones we'd rather it hadn't learned. Hold onto that thought. It's where chapter 3 begins.

## So what is it actually good for?

A great deal, once you understand what you're working with. Because it's a pattern machine, an LLM is genuinely strong at pattern work: rephrasing something you don't understand, summarising a long text, translating, generating questions to test yourself with, suggesting ideas when you're stuck.

What it can't do is care whether it's right, know what your teacher actually taught you, or take responsibility when it gets things wrong. Checking, questioning and deciding what to trust is your job. The rest of this guide is about doing that job well.

[Panel, chapter closer.]

## 3 takeaways

1. **An LLM predicts, it doesn't know.** There's no database of facts behind it, just patterns learned from human writing.
2. **Probable is not the same as true.** It states falsehoods with the same fluency and confidence as facts.
3. **It learned from people.** Our best thinking and our worst assumptions went into the training data together.
