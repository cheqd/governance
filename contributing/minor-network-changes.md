# Minor Network changes

## **Minor Network changes**

These are changes that are insignificant, and do not affect the way the Network runs overall. Minor Network changes include, but are not limited to:

* Textual edits to the Governance Framework or written general documentation;
* Sensible additions to general documentation to improve clarity;
* Minor code changes;
* Finding, reporting and suggesting fixes to bugs;
* Translating the cheqd documentation into various languages.

## Decision tree

To help YOU understand how to make changes on the cheqd Network, the decision tree below visualises how changes should be carried out.

![Decision tree for Network Governance](<../.gitbook/assets/On-chain vs off-chain decision tree.jpg>)

## Voting off-chain

One of the core components of cheqd governance is having both on-chain and off-chain voting mechanisms.&#x20;

Off-chain voting should be used for Minor Network Changes as well as for more general community polling.

cheqd uses the Governance platform Commonwealth to enable off-chain votes on specific forum discussion topics.

{% embed url="https://commonwealth.im/cheqd" %}

We will point the community to off-chain votes using our Telegram and Discord to keep all of the community in the loop.

## How do I make edits to general text or code in cheqd documentation?

You are able to make revisions and amendments to the Wiki and source code without making a formal Proposal.

cheqd is an Open Source project which means that anyone is free to propose or make a revision, addition or amendment.

Changes can be made through two routes:

1. [GitBook](https://docs.cheqd.io/governance/)
2. [GitHub](https://github.com/cheqd)

### GitBook

GitBook is where cheqd's Wiki lives and where YOU can make suggested changes to the written documentation.

We suggest that YOU use our GitBook if you are unfamiliar with GitHub or if you prefer visual editors to code-based editors.

We have a Wiki for:

1. [cheqd Technical documentation](https://docs.cheqd.io/node/)
2. [cheqd Governance Framework](https://docs.cheqd.io/governance/)

To make a change on either Wiki, you need to use the link below to become an Open Source Editor on cheqd's GitBook:

{% embed url="https://app.gitbook.com/invite/-MiQSPMufVJdYEwQHd2c/t69fUvhwkQVP4MeOEE1e" %}

Once you have made your account using the link above, you will be classified as a [Editor](https://docs.gitbook.com/collaboration/team-management/setting-up-permissions) on cheqd's GitBook. This will give you the ability to make edits and submit them to be reviewed by a [Reviewer](https://docs.gitbook.com/collaboration/team-management/setting-up-permissions). Reviewers are able to merge submitted changes.

You should follow these instructions to make a edit to any cheqd GitBook content.

1. **Make your edits in the text directly or use comments**\
   Via the link above, you will gain permissions to to read, edit and comment directly to the text.\
   \
   If you are confident with your edits, you can write and amend the text directly. If you are less confident, you can leave comments in the text, which admins will review and make changes from accordingly.\\
2.  **Save your changes as a draft**

    ***

    You can save your changes as a draft and return to your draft later. If you want to remind yourself with the changes you made previously, you should click the Diff view button:

![](<../.gitbook/assets/image (1) (1) (1) (1).png>)

You should keep your changes in drafts until you are happy with them.

\
Following this as best practice, avoids the Wiki being misused or flooded with changes from one person.

3\. **Submit your changes**\
\
Once you are happy with your changes in your draft you should click Submit. This will send your changes to one of our Reviewers to be moderated before being pushed onto the documentation.

There will be a pop-up asking you to explain the changes you made. Make sure to write a clear sentence summarising your main changes to make it easier for the cheqd reviewers to go through your work.

### GitHub

You may also use GitHub to make changes and amendments to both the source code and the written content in this documentation.\
\
We have multiple GitHub repositories which can all be accessed [here](https://github.com/cheqd).\
\
For instructions about making edits to GitHub repositories, we suggest you follow the instructions [here](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files).

**Please use clean, concise titles for your pull requests.** Assume that the person reading the pull request title is not a programmer, but instead a cheqd Network user or lay-person, and **try to describe your change or fix from in plain English**. We use commit squashing, so the final commit in the main branch will carry the title of the pull request, and commits from the main branch are fed into the changelog. The changelog is separated into [keepachangelog.com categories](https://keepachangelog.com/en/1.0.0/), and while that spec does not prescribe how the entries ought to be named, for easier sorting, start your pull request titles using one of the verbs "Add", "Change", "Deprecate", "Remove", or "Fix" (present tense).

Example:

| Not ideal                            | Better                                                        |
| ------------------------------------ | ------------------------------------------------------------- |
| Fixed NoMethodError in RemovalWorker | Fix nil error when removing statuses caused by race condition |

It is not always possible to phrase every change in such a manner, but it is desired.

**The smaller the set of changes in the pull request is, the quicker it can be reviewed and merged.** Splitting tasks into multiple smaller pull requests is often preferable.

**Pull requests that do not pass automated checks may not be reviewed**.

## Bug reports

During the course of cheqd's lifecycle, it is likely that bugs will arise. Reporting these bugs effectively and resolving them promptly will be very important for the smooth running of the Network.

Bugs can be discussed or raised in our [Telegram](https://t.me/cheqd) or [Discord](https://discord.gg/s4nuefbY).&#x20;

If there is common acknowledgement of the bug, next the bug SHOULD be highlighted as an issue in our forum, at:

{% embed url="https://commonwealth.im/cheqd" %}

Please use the search function to make sure that you are not submitting duplicates, and that a similar report or request has not already been resolved or rejected.

## Translations

We would greatly appreciate this work from our community to ensure that cheqd reaches a diverse, multijurisdictional and multilingual spread of society!

We are currently working on a simple process for submitting translations through a GitHub branch. Please bear with us until we figure out a simple way to achieve this!
