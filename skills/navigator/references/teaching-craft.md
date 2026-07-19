# Teaching craft

Read this when a gate, a wrong answer, or a stuck debugging moment needs to be better than
routine. It covers only the moves that aren't already in SKILL.md and that are easy to get
wrong — not a rationale for the protocol, and never material to recite at the user.

## Writing gate questions

Ask for the counterfactual ("what breaks if…"), the failure mode, the trade-off, or the
boundary condition — anything that forces reconstruction from the model rather than recall of
a phrase. A definition can be recited by someone who understands nothing; a wrong prediction
cannot be faked. Anchor questions to their actual artifact and to concrete states ("record 400
of 500 fails to write — what does your code do with 401 through 500?") rather than to the
concept in the abstract. And "does that make sense?" measures nothing: learners systematically
overrate their grasp of material they have just read (Bjork, Dunlosky & Kornell, 2013), so
self-report is the one signal to ignore.

## When they get it wrong

A confidently wrong answer is the most valuable outcome available — errors made with high
confidence are, once corrected, the best-remembered corrections of all (the hypercorrection
effect; Butterfield & Metcalfe, 2001). Say that plainly instead of softening the miss. The same
logic makes a failed pretest guess worth inviting before a primer.

But note the mechanism, because it constrains the Socratic rule: the benefit comes from the
correction *landing*, not from the error alone. Withholding a diagnosis while they still have
hypotheses is right; leaving a confident error uncorrected after they have stopped generating
wastes the best moment you get.

## Debugging

What is actually being learned is hypothesis-testing under uncertainty — predict, gather
discriminating evidence, eliminate. That transfers across every stack they will ever touch,
which is why it is worth protecting more than any particular bug's fix. When they are stuck,
useful help is a new *generative* move — flip the search direction ("assume the compiler is
right: what disaster is it preventing?"), or name what their two dead hypotheses already
eliminated — not a clearer restatement of the error.

Withholding the answer can beat immediate feedback for retention, which is the case for
Socratic debugging, but the evidence is genuinely mixed: lab studies tend to favor delayed
feedback (Butler, Karpicke & Roediger, 2007) while classroom studies often favor immediate
(Kulik & Kulik, 1988). So there is no principled reason to grind. Once they are out of
hypotheses, delay has stopped buying anything — offering the escape hatch is the honest move,
not a failure of the mode.

## Never ask what kind of learner they are

Matching instruction to a claimed learning style has no demonstrated benefit (Pashler,
McDaniel, Rohrer & Bjork, 2008). Home-territory analogies work because they are prior
knowledge, not because of a style preference — so establish what they already know, never how
they prefer to be taught.

When in doubt, the move with the best evidence behind it is the same one every time: make them
retrieve it.
