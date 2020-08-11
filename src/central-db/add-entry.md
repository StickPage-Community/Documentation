---
description: Adding an new entry? This page will help
---

# Adding new entry

{% hint style="info" %}
Before adding a new entry, please take some time to [read the documentation on our JSON Schema](schema/).
{% endhint %}

## Requirements

The following are mandatory when submitting a new entry to the database.

* **Has a thread entry for applications in** [**StickPage Forums**](http://forums.stickpage.com/forumdisplay.php?51-RHG-Characters) **or** [**Hyun's Dojo Forums**](https://www.hyunsdojo.com/community/viewforum.php?f=47)**.** We can't search around these forums just to look for the application thread. Please give us the link. No link shorteners, please
* **Has a YouTube channel.** THIS IS VERY IMPORTANT for identity verification purposes.

### Recommended but optional

* **Has a GitHub or GitLab account with at least 10 contributions in the past 14 weeks.** Nah, we don't care about your contributions count, just checking if you're active in the open-source community.
* Has other social accounts such as Twitter and Patreon. Not only this improves our identity verification process, but also

## Getting started

### Your own stick character

Before we can process your request, make sure that you started your [RHG](https://web.archive.org/web/20191104230834/http://forums.stickpage.com/showthread.php?33615-Starting-your-RHG) and/or [Duelist](http://www.hyunsdojo.com/community/viewtopic.php?f=47&t=6178). Only one character can be added to the database per person. If you want to add more, [see this FAQ entry](add-entry.md#i-want-to-add-2-or-more-stick-characters-i-make-is-it-allowed).

If you're ready to continue, [skip to the process section](add-entry.md#the-process).

### Somebody's stick character

{% hint style="info" %}
**Updating or removing an entry?** See [Updating current entry](updating-entry.md) or [Removing an entry](remove-entry.md) for details.
{% endhint %}

Before adding a stick character that made by someone, please check for any active merge requests in both GitHub and GitLab relating to it. If you found one, it better to join the discussion instead of creating a new one to keep our backlog clean.

## The Process

### TL;DR

* Fork this repository [in GitLab](https://gitlab.com/stickpage/Database-Repository/-/forks/new) \(or [in GitHub](https://github.com/StickPage-API/Central-DB/fork)\).
* \(optional\) Clone your fork locally or open it in Gitpod.
* Copy the `templates/stickpage-entry.json` file to `stickpage/<your-entry-here>.json`, replacing `<your-entry-here>` with your entry name in a URL-friendly style.
* Fill up the fields as possible as you can. After filling up the fields, also

```text
<!---
Append these on the last line of either .github/CODEOWNERS,
.gitlab/CODEOWNERS, or both (only if you use both GitHub and GitLab.com).
-->

stickpage/stick-character-name-here.json @YOURGHORGLUSERNAMEHERE
animators/animator-name-here.json @YOURGHORGLUSERNAMEHERE
```

* Sign-off your commits \(and optionally sign it using your GPG key\) and push to your fork.
* Create a new merge request and follow the discussion.

## FAQ

### I want to add 2 or more stick characters I make. Is it allowed?

As per current policies, each person can only request ONLY ONE character to be added to the database. If you want to add more than 2 characters you made, please let others add it for you.

If you REALLY WANT to add more, you may edit or remove your current entry as you wish.

### Why my entry was rejected?

If one of our maintainers or

```text
Hi <username>,

Your entry addition was rejected by our maintainers due to the following reason:

[reason here]

If you think this is wrong, please see [this FAQ entry] in the documentation
for more information on how to troubleshoot this issue.

[this FAQ entry]: https://thepinsteam.gitbook.io/stickpage-api-docs/central-db/add-entry#why-my-entry-was-rejected

Your next commit must contains the following text below so we can re-review your
changes as soon as possible.

```
[fix-issues] Resolved entry rejected on Request ID 1234-ABCD-56-EF

This commit was requested by the maintainers, as per [link to this comment]

Signed-off by: [author name <username@example.com>]
```

Regards,
[maintainer's name or the username of the service account]
```

Possible reasons are:

* **Your entry doesn't have enough data.** Please fill up the fields as possible as you can.
* **The link/s don't work anymore.** Make sure links are working. If not, attempt to fix it or use the Wayback Machine link.
* Not up to the standards. 

