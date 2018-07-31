# Agile Estimation

For software developers, estimation is among the most difficult–if not the most difficult–aspects of the job. It must take into account a slew of factors that help product owners make decisions that affect the entire team–and the business. With all that at stake, it's no wonder everyone from developers to upper management is prone to getting their undies in a bunch about it. But that's a mistake. Agile estimation is just that: an estimate. Not a blood-oath. 

There's no requirement to work weekends in order to compensate for under-estimating a piece of work. That said, let's look at some ways to make agile estimates as accurate as possible.  

## Collaborating with the product manager

In agile development, the product manager is tasked with prioritizing the backlog–the ordered list of work that contains short descriptions of all desired features and fixes for a product. Product owners capture requirements from the business, but they don’t always understand the details of implementation. So good estimation can give the product manager new insight into the level of effort for each work item, which then feeds back into their assessment of each item's relative priority.

When the engineering team begins its estimation process, questions usually arise about requirements and user stories. And that's good: those questions help the entire team understand the work more fully. For product managers specifically, breaking down work items into granular pieces and estimates via story points helps them prioritize all (and potentially hidden!) areas of work. And once they have estimates from the dev team, it's not uncommon for a product owner to reorder items on the backlog. 

## Agile estimation is a team sport

Involving everyone (developers, designers, testers, deployers... everyone) on the team is key. Each team member brings a different perspective on the product and the work required to deliver a user story. 

For example, if product management wants to do something that seems simple, like support a new web browser, development and QA need to weigh in because their experience has taught them what dragons may be lurking beneath the surface.

Likewise, design changes require not only the design team's input, but that of development and QA as well. Leaving part of the broader product team out of the estimation process creates lower quality estimates, lowers morale because key contributors don't feel included, and compromises the quality of the software.

Note, there is evidence that shows that estimation accuracy drops off significantly beyond one day’s work. We, as humans, are pretty good at estimating the amount of work we can complete in a single day but our accuracy drops off dramatically the more days are required. 

So don’t let your team fall victim to estimates made in a vacuum. It’s a fast track to failure! 

## Story points vs. hours

Traditional software teams give estimates in a time format: days, weeks, months. Many agile teams, however, have transitioned to story points. Story points rate the relative effort of work in a Fibonacci-like format: 0, 0.5, 1, 2, 3, 5, 8, 13, 20, 40, 100. It may sound counter-intuitive, but that abstraction is actually helpful because it pushes the team to make tougher decisions around the difficulty of work. Here are few reasons to use story points:

```

Dates don’t account for the non-project related work that inevitably creeps into our days: emails,
meetings, and interviews that a team member may be involved in.

Dates have an emotional attachment to them. Relative estimation removes the emotional attachment.

Once you agree on the relative effort (High, Medium, Low) of each story point value, you can assign points quickly 
without much debate.

Story points reward team members for solving problems based on difficulty, not time spent. This keeps
team members focused on shipping value, not spending time. 

```


## Story points and planning poker

Teams starting out with story points use an exercise called planning poker. The team will take an item from the backlog, discuss it briefly, and each member will mentally formulate an estimate. Then everyone holds up a card with the number that reflects their estimate. If everyone is in agreement, great! If not, take some time (but not too much time–just couple minutes) to understand the rationale behind different estimates.

The reason to use planning poker (PP) is to avoid the influence of the other participants. If a number is spoken, it can sound like a suggestion and influence the other participants' sizing. Planning poker should force people to think independently and propose their numbers simultaneously. This is accomplished by requiring that all participants show their card at the same time.



## Estimate smarter, not harder

No individual task should be more than 16 hours of work. (If you're using story points, you may decide that, say, 20 points is the upper limit.) It’s simply too hard to estimate individual work items larger than that with a high degree of confidence. And that confidence is especially important for items at the top of the backlog. When something is estimated above your team's 16-hour (or 20-point) threshold, that's a signal to break it down into more granular pieces and re-estimate.

## Learn from past estimates

Retrospectives are a time for the team to incorporate insights from past iterations–including the accuracy of their estimates. 

Many agile tools (like Jira Software) track story points, which makes reflecting on and re-calibrating estimates a lot easier. Try, for example, pulling up the last 5 user stories the team delivered with the story point value 8. Discuss whether each of those work items had a similar level of effort. If not, discuss why. Use that insight in future estimation discussions.

There are some good arguments against doing task estimation. For some high-performing teams, it can be worthwhile to avoid the exercise, especially if the team has demonstrated good accuracy in the past. And for teams that are doing Scrumban or some other pull-model process, the goal is to move toward similarly-sized stories to help facilitate flow.

Like everything else in agile, estimation is a practice. You'll get better and better with time.


# The Fibonacci sequence in agile

When estimating the relative size of user stories in agile software development the members of the team are supposed to estimate the size of a user story as being 1, 2, 3, 5, 8, 13.

Several commercially available decks use the sequence: 0, ½, 1, 2, 3, 5, 8, 13, 21, 34, 100, and optionally a ? (unsure), an infinity symbol (this task cannot be completed) and a coffee cup (I need a break, and I will make the rest of the team tea). Some organizations[which?] use standard playing cards of Ace, 2, 3, 5, 8 and king. Where king means: "this item is too big or too complicated to estimate". "Throwing a king" ends discussion of the item for the current sprint.

Smartphones allow developers to use mobile apps instead of physical card decks. When teams are not in the same geographical locations, collaborative software can be used as replacement for physical cards.

### Procedure

At the estimation meeting, each estimator is given one deck of the cards. All decks have identical sets of cards in them.

The meeting proceeds as follows:

```
1. A Moderator, who will not play, chairs the meeting.

2. The Product Owner provides a short overview of one user story to be estimated. The team is 
given an opportunity to ask questions and discuss to clarify assumptions and risks. A summary of 
the discussion is recorded, e.g. by the Moderator.

3. Each individual lays a card face down representing their estimate for the story. Units 
used vary - they can be days duration, ideal days or story points. During discussion, 
numbers must not be mentioned at all in relation to feature size to avoid anchoring.

4. Everyone calls their cards simultaneously by turning them over.

5. People with high estimates and low estimates are given a soap box to offer their justification
for their estimate and then discussion continues.

6. Repeat the estimation process until a consensus is reached. The developer who was likely to own 
the deliverable has a large portion of the "consensus vote", although the Moderator can 
negotiate the consensus.

7. To ensure that discussion is structured; the Moderator or the Product Owner may at any point 
turn over the egg timer and when it runs out all discussion must cease and another round of poker 
is played. The structure in the conversation is re-introduced by the soap boxes.

```


## Benefits 

Breaking down stories into “right-sized” tasks also has several benefits:

1. The right level of granularity. When we break a story into tasks, it helps ensure that the team is asking the right questions of the Product Owner to understand what’s needed to deliver on it. It’s critical that the team have a good starting point for their work.


2. Covering all the bases. A good practice is to do this exercise as a team. With a good cross-functional team, they should work together to identify all the steps needed to complete the story. It should cover all development, testing, and validation work needed.


3. Incremental progress. By completing stories in small steps, the team can show progress toward their sprint goals.


4. Burn-down charts. Using hours to track our burn-down charts (as opposed to story points) can provide more detail on our sprint progress.

