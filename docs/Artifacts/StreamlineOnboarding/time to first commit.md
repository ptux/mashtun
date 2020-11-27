# [WIP] Time to First Commit

It’s the time it takes
from when The New Person turn on PC
to the time when they've pushed the first commit to the version control system.

## It’s Comprehensive

developer

- organization’s Software Development Life Cycle polices
- a task in issue tracking system
- security credentials
- a fully configured development envrioment
- source code from the version control system

## It’s Quantitative

Time to First Commit is a measurable quantity, which means that it’s relatively easy to figure out where your team is at now, what a reasonable target might be, and then steps the team can take to drive towards achieving that goal. It means that as new tools are adopted and processes evolved over time, you can measure whether these things have positively or negatively impacted this metric and take the necessary steps to address any problems. For example, if a developer checks in a change that brings in some new dependency and hasn’t documented how to set it up (or better yet, automated the setup), it’s pretty likely you’ll see a regression in this metric.

## Optimizing For Time to First Commit

Documentation:

- Development environment setup guide.
- Makefile target descriptions. 
- Instructions for running both unit and end-to-end tests
- Recommended tools, editor plug-ins, etc.

Automation:

- CI
- Git hooks
- Makefiles

