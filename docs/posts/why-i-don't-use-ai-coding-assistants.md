---
date: 2025-04-13
categories:
  - AI
---

# Why I don't use AI coding assistants

During the last few months, I have been trying pretty much all the AI coding assistants
available and the different ways to engage with them.

A couple of weeks ago, I finally reached the *radical*? conclusion that I will not use them at all.

I see a lot of polarized discussions online focusing on the perceived *performance* of these systems,
which is why I wanted to discuss at least a couple of points where that aspect is irrelevant.

I hope to stand by my decision even if/when the assistants become actually good.

<!-- more -->

---

During these months, I have confirmed and experienced different **negative** effects of using
AI assistants.

I tried to group those negative effects under 4 different categories:

- [Environmental](#environmental)
- [Social](#social)
- [Personal](#personal)
- [Professional](#professional).

!!! info

    It is not my intention to put shame on people using AI coding assistants.

    I, too, use tools and take actions every day that have negative effects,
    it's just that in this particular case the benefits for me (if any) were
    not even close to outweigh the sum of negative effects.

## Environmental

The companies behind these systems have managed to (almost?) completely hide from the public scrutiny the environmental impact behind that line completion that you end up discarding or that Pull Request review that ends with "no comments".

They've carefully designed an UX to hide what is happening under the hood,
trying to make you believe that it requires similar compute to similar tools you are used to (like that lovely optimized linter written in Rust).

!!! danger

    My environmental concerns were already present using the lightest form of ai assistance (auto-completion).
    More recent approaches like agentic assistants just multiply these concerns.

There is no room for techno-optimism.

AI companies will never focus on making the overall system more environmentally friendly. They'll keep releasing new
hardware and software versions only to train and serve even bigger models.

Along the way, they keep consuming an ever-increasing ridiculous amount of resources and leaving behind electronic waste from which we will be never able to fully recover.

We should (at the very least) push back on the uses cases were we don't see value.

## Social


I feel that AI coding assistants are negatively affecting our shared knowledge in much more subtle ways than some obvious
effects (like AI crawlers tearing down the infra behind that shared knowledge) .

Not happy with using our shared knowledge without proper attribution/compensation, AI coding assistants today are carefully
designed to isolate the user from the original sources of knowledge.

!!! danger

    Ironically, the AI coding assistants seem to incentivize the contamination of those original sources of knowledge in the form of fake content, hallucinated bug reports, auto-generated code repositories, etc.

Before these tools, everyone was incentivize to be an active participant of this knowledge sharing:

- When searching for an answer in Stack Overflow, people could participate in many different ways: upvote the most useful one, comment to improve an existing answer, create a new question, etc. When copy-pasting some code, you were **consciously** deciding to acknowledge the source or not.

- When using an open-source project and missing a feature or facing a bug, you would search the docs, ask in the forums, try to contribute with code or documentation updates, etc.

But now, with AI coding assistants:

- When you get some generated code, there is no indication of where it came from, no room for discussion with others, etc.

- When you hit a bug in a library, you just ask for a fix, a workaround, or an alternative library. There is no feedback loop going back to the maintainers of that library nor sharing of your findings with others.

## Personal

I see a lot of people saying they love AI coding assistants because it's helping them build complete
side projects at an incredible pace. I feel happy for them but at the same time a little worried.

!!! question

    At which point people started to enjoy "achievements" (finishing a project) if there was no
    real effort behind (just prompting Firebase Studio with a vague idea)?

My joy when working on side projects comes from the process itself of learning something new, putting
the time to go through the most unexpected rabbit wholes, etc.

It was never about accumulating finished projects and I don't want to be dragged into that "race".

## Professional

The open source ecosystem is full of remarkable projects that were written by empathic humans before the existence of AI coding assistants, which have been trained to memorize all of them (along with some less remarkable ones).

How is it possible that, in my several months trying AI coding assistants, I felt that I was becoming a little worse engineer every week?

!!! info

    I am currently working with very recent projects (i.e. agentic frameworks) so I can understand
    how assistants struggle with things they didn't memorize.

    I tried to not be biased despite the fact that any of the "traditional" tools (i.e. linters, type-based completion)
    and/or processes (opening a github issue or ask in a forum) already work out of the box no matter if the
    project was released yesterday.


### Lack of empathy

I reached a critical point when I was git blaming "who the fuck wrote this shitty docstring and tests" only to
find that it was me, a week before, using a "state of the art" AI coding assistant.

It was not only the fact that they were useless, it was more about me having accepted those suggestions as good and
forgetting about it.

I went to look at some docstrings and tests I wrote 10 years ago in one of my first Python projects, and felt
really ashamed finding them objectively more useful.

Without barely noticing, I was dragged by the AI assistant into a world where things like docstrings and tests are just checkboxes to make the linter/reviewer happy, instead of critical parts to improve the life of the ones that will come
after.

For me, good software is about empathy with the future readers/users (including yourself) of the code, docs, and tests.

If AI coding assistants today couldn't learn that pattern after seeing every remarkable open source software available, how will future versions improve when everyone is bloating the public domain with unemphatic AI-generated projects.

### Hiding the root issues

One of the use cases I found most promising was using assistants to review Pull Requests.
I got a couple of useful comments in the first tries and though: well, it seems slightly better than a linter.

However, after a couple of more reviews, I started to realize that any actually useful comment was only possible
because there was a much bigger issue behind, like lack of test coverage or missing some rules in the linter.

Again, the assistant was dragging me into a world were I was incentivize to forget about fixing the root issues
(like taking some time to improve the CI workflow) and instead over-relay on a tool to hopefully catch some of the
visible consequences (if you get lucky with the RNG).

## Conclusion

I want to acknowledge the possibility that I might just be a low-taste, lazy-prompter who approached
every AI coding session with the wrong *vibes*.

Nevertheless, I will be in peace with myself if everyone digivolves into AI-augmented-engineers
and I become the liability.
