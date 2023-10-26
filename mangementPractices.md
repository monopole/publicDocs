# Software Engineering Management Practices

This doc is meant to be a high level summary of
practices that I've seen work in software engineering
management, and have thus adopted in my own behavior.

It might save time to read this before engaging with me
on some topic related to SW Eng management.

[readmes]: https://meakaakka.medium.com/a-beginners-guide-to-writing-a-kickass-readme-7ac01da88ab3
[Pair program]: https://martinfowler.com/articles/on-pair-programming.html

[deprecate yourself]: #deprecate-yourself

## Deprecate Yourself

The best engineers solve problems and move on.

Ways to deprecate yourself:

* Write clear problem statements.  Before engaging in
  _"solutioning"_, be sure that you've articulated a
  problem in written form and sought feedback from
  others.  This is the most important skill for an
  engineer to practice and improve on.

* Write other material - solution proposals, [readmes],
  code comments, blog posts, drive-by edits to wiki
  pages, etc.

* Write tests that stand guard against regressions as
  people build on your work.

* Make long term plans - be ready to describe where
  your projects should be going and not going.

* Give recorded talks.

* If you're a frequently used point of contact for
  something, convert that into an on-call rotation
  responsibility.

* [Pair program].


Don't be the person who builds some inscrutable
collection of bash or python scripts in an attempt to
achieve job security.

## The 1:1

The purpose of a 1:1 meeting is to help each other as
colleagues.

If there's something you need help with, or want to
escalate, bring it up.

Provide _updates on tasks_ if it helps get the ball
rolling, but as a team we have other, better means to
surface progress on work - standups, bug tracker
summaries, kanban boards, release notes, etc.


## Process

A good process is a set of _team habits_ that minimize
_decision fatigue_, clearing the path to productive
execution.

A good process defines a means _within itself_ to
change itself.

Good habits:

* periodic review of new problems, priorities, and ongoing tasks
* periodic demos, releases and expressions of gratitude
* test writing, often as a first step to coding
* sprints

Having sprints is different from, say, just writing a
bunch of code for months on end.

A sprint is a fixed time period where engineers pull
from a prioritized list of well defined tasks and
execute them in a state of flow uninterrupted by
uncertainty and doubt.

This implies thought was invested in defining and
ordering thje list to serve some user need.  Ideally
such a list is made by a product manager (PM), with
input from users and  engineers.

The sprint end date provides a pause opportunity for
several things:

* Ship a new release.

  This is a good idea even if no new user-visible
  feature is shipped, because _something_ changed,
  e.g. a version bump in a deeply-transitive backend
  library.

  We don't want such changes to build up over time
  without being tested and shipped because deep bugs
  will just be that much harder to track down.

  Related - don't do development in feature branches that
  require some massive merge commit.

  Commit _all code to main_, but hide features behind
  enablement flags.

* Have a retrospective meeting to consider changing process.

  Process-change decision points must be infrequent.
  Frequent change is indistinguishable from no process.

  A process change must have enough time, at least one
  sprint, to show its effectiveness.  Changing more
  than one or two things at a time can be exhausting
  and inconclusive.

  Process-change decision points are so important that
  they, not releases, define the _overall periodicity_
  for the process.

* Free up engineers to help the PM refine the next
  sprint.

* Optionally, have a few hack days. etc. etc.


## Roles

In general, a Product Manager must know why, a Project
Manager must know when, an Engineer must know how, and
the QA team, if any, knows what's actually done.

If you don't have QA, then work with the PM to define
_done_ before implicitly and unprofessionally asking
users to determine that for you when push out a
release.

Roles assure that _decisions are taken in their areas of
concern_.

Use [process](#process) to make this easier for everyone.


## Decisions

Decisions must be made to move forward.  It's better to
proceed on a "wrong" decision - and learn from it and
maybe reverse it as a result - than to languish.

If a decision doesn't go your way, there's a short
window (short relative to the time taken to arrive at
that decision) in which you must do one of the
following:

- Escalate to your manager or manager's manager to get
  the decision reconsidered at a higher level.

- Adjust your mindset to help make it work despite your
  objections.

- Actively _get out of the way_ by arranging to work on
  something else - there's always plenty to do.


## Journaling

Maintain a daily, or at least weekly, _journal_ of what
you do.

If possible, make it publically readable and searchable (within the
company) but even if that's not possible write it _as if_ it will be
published.

[logseq]: https://logseq.com
[obsidian]: https://obsidian.md


Some options:

* A text file stored in an internal git server.
* [logseq] (with an internal git server).
* [obsidian] (ditto).
* Some internal document cloud (sharepoint, wiki, etc.)

This helps one align the relatively small tasks of the
day with overall team and company goals.

This is an opportunity to make note of things you are
doing that are not part of the work flow coming from a
sprint, e.g. interviews, intern mentoring, tuning up
some wiki pages, hunting down a network problem at the
workplace, arranging an off-site, etc.

[performance summaries]: #performance-summaries

## Performance Summaries

At performance review time, you will be asked to
provide a summary of your achievements for some time
period, usually a quarter or two.

Do not assume that your manager can or will track this.

It's common to work hard for six months, keep the boat
afloat, row frantically towards some destination, but
at the end of this time stammer when asked what you
did.

[Journaling](#journaling) solves this problem, as well
as other problems.


## Promotion

An important role for a manager is to match direct
reports with opportunities that can showcase their
development.

To get help with this, try to pin down what your
strengths are, and what areas need help.

If you want a promotion,

* Decide a quarter or two in advance.

* Assume a _higher than normal_ quality bar for the
  [performance summaries] written in those quarters.

The information in those performance summaries must be
understandable to someone unfamiliar with your work.

It needs to be understandable to others managers who
engage in _promotion calibration_. The managers are
looking at promotion candidates across teams and trying
to compare them to job-level role descriptions.



## The Next Level

Doing _work_ is a necessary and sufficient condition to
being a good team member and remaining at level
collecting compensation.

Don't confuse compensation and promotion.

A promotion is not a _reward_ for work.

A promotion is recognition that you are currently
meeting the expectations of the next level, and that
this should be made official.

To get promoted you must be able to provide written
evidence via [performance summaries] of performing at
level _N+1_. Doing so helps your manager make your case
to others.  Not doing so is evidence that you aren't
ready for promotion.

A promotion might not significantly change your
compensation, because you should be moving from a
_greatly-exceeds-expectations_ at level _N_ to a
_meets-expectations_ at _N+1_.


### Becoming a Manager

A "promotion" that involves a switch to management is a
significant role change.

It's widely recognized that being a great individual
contributor (IC) is not correlated with being a great
manager.

Many engineering organizations have worked to make
distict tracks for IC and management, and provide a
means to switch back and forth between these tracks.

You'll have to [deprecate yourself] from the bulk of your IC
work to become an effective manager.


## Vacations

Obviously, it benefits you to take a break.  Get your head above the
canopy and look across the forest to the horizon.

It also benefits the team as they get a chance to fill your shoes and
become stronger for it.  It's a concrete opportunity to
[deprecate yourself].
