---
layout: post
title: Value of deduplication moderation for user submissions
---

Building on the framework in [Comment ranking formulas](/2020/05/21/comment-ranking/),
if we add a new positive integer parameter called `max_unique_comments`, and we say that new comments are drawn uniformly at random from the set of unique comments with cardinality `max_unique_comments`, now users' experiences with a comment depend on comments they're previously seen. Using the Modified Bayes scoring system, we see the following results.
Assume the comment section lasts for 24 hours, there are 10 visitors per hour, and the probability that a visitor makes a comment is 0.1.

If `max_unique_comments` is 12: 
* If duplicate comments are removed immediately, the average number of upvotes per visitor is 0.65
* If users downvote any comments they've seen before, the average number of upvotes per visitor is 0.62
* If users downvote any duplicate comments they see that don't have the highest difference upvotes - downvotes, the average number of upvotes per visitor is 0.63

If `max_unique_comments` is 18: 
* If duplicate comments are removed immediately, the average number of upvotes per visitor is 0.73
* If users downvote any comments they've seen before, the average number of upvotes per visitor is 0.70
* If users downvote any duplicate comments they see that don't have the highest vote difference (upvotes - downvotes), the average number of upvotes per visitor is 0.71

So in conclusion: There is value in removing duplicates manually, not just leaving it up to the voting system.

Code: <https://gist.github.com/andrew222651/cc32d857d9078f38a7b4c4b70c74ff51>
