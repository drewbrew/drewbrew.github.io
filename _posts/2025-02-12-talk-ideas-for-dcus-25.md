---
title: "Things I'd Like to See in a DjangoCon US 2025 Talk"
published: true
---

In [previous](https://2023.djangocon.us/news/topic-suggestions-for-cfp/) [years](https://2022.djangocon.us/news/topic-suggestions-for-cfp/), I've written suggestions for what topics might be good in a DjangoCon US talk. Last year, I [wrote](/2024/03/01/talk-ideas-for-dcus-24/) some suggestions on my personal blog. As I'm no longer the Program Chair, I'm doing the same this year.

So, here's a rough list of talks I'd like to see submitted in [this year's CFP](https://pretalx.com/djangocon-us-2025/cfp), which is open until April 27. Submitting one of these won't guarantee you a slot in the program, but it can't hurt! This year, I'll be anonymizing the talks before reviewers get their hands on them.

Some of these are tweaks from last year (they're still good topics, [Brent](https://knowyourmeme.com/memes/theyre-good-dogs-brent)), and some are new. Enjoy!

## Developing for good in the current political climate

Let's face it, things in the US suck right now. We have more constitutional crises going on than we have days of the week it seems. How do we use our tech skills to make the world a better place, especially those whom the current administration is targeting?

## Deep dives into the internals of Django and related libraries (e.g. REST Framework)

Have you ever had something that was acting in an unexpected manner and then you dug deeper into the source and exclaimed to yourself, "aha! This is how (and why) it works!" Share those insights! Bonus points if it's something relatively new to Django.

## Ok, you made the polls app. Now what?

Think of this as a tutorial part 2. You've created the simple tutorial app running locally. What do you need to do to convert that into a full-scale webapp in 2025? Think of this as a spriritual sequel to Katie McLaughlin's [What is deployment, anyway?](https://2021.djangocon.us/talks/what-is-deployment-anyway/) talk from 2021.

## New features in Django 5.2 (or better yet, 6.0!)

Django 5.2 is slated to be released in April 2025, which is right on time for the CFP. However, [Django 6.0](https://docs.djangoproject.com/en/dev/releases/6.0/) is scheduled for December 2025, which means you can draft your CFP based on what is currently in main and adjust it to the alpha/beta releases as needed before the conference itself.

## Introducing the Django 6.x Steering Council

Granted, this talk could only come from [5 people](https://www.djangoproject.com/weblog/2024/dec/18/django-6x-steering-council-election-results/), but this would be an excellent opportunity to share your goals for the Django project, your hopes and dreams, and how your leadership fits into the overall vision of Django and how the community can help.

## Challenges of using a project like Django in a world where single-page apps (SPAs) are the norm

Yes, HTMX and the like are seeing a nice bit of developer mindshare, but you're not going to change the minds of people who have spent the past decade-plus immersed in a JS-first world overnight.

## Unexpected use cases, especially ones that make the world better

These are some of my personal favorites. I love reminding people that yes, we're a tech conference, but overall, the tech is supposed to serve the people, not the other way around.

## Clever hacks (such as Carlton Gibson's [single-file Django project](https://2019.djangocon.us/talks/using-django-as-a-micro-framework-on-the/))

Do you like absurd uses of Django? Python? Share them! Sometimes the insights you gain by doing things in a completely unorthodox manner are the ones that spur all kinds of weird discussions and possibly even some innovations. Richard Terry's nanodjango lightning talk from last year would be a great full-length talk this year!

## No GIL, No Problem? How Python (possibly) removing the Global Interpreter Lock might affect your Django app

[PEP 703](https://peps.python.org/pep-0703/) was released as part of Python 3.13 as a build-time option `--disable-gil`. It'll be a long time before this becomes the default, especially because Django doesn't currently work under a nogil setup, AFAIK. Give a deep technical look at how we can bring Django forward into this new era, and you might even spawn some [DEPs](https://docs.djangoproject.com/en/5.1/internals/contributing/writing-code/submitting-patches/#django-enhancement-proposal-dep) in the process!

## HTMX/Alpine/Tailwind/other new CSS/frontend framework

We typically have a couple of these each year. They're a big draw and really help a lot of people.

### Related: integrating channels into an HTMX project for even more responsiveness/interactivity

Have you used channels for websockets?  How about using them with an HTMX project?

## Development and testing techniques that help you build better code

I thought [Marc Gibbons' talk](https://2023.djangocon.us/talks/empathetic-testing-developing-with-compassion-and-humility/) on empathetic testing really did a good job of explaining how to make life easier on your fellow devs (and also be more understanding when things inevitably go wrong). I'd love to see a talk this year expounding on that theme and taking it deeper and broader.

## Philosophical debates around code architecture, such as [when to make the call on a large-scale refactor](https://2017.djangocon.us/talks/live-long-and-refactor/)

As developers, we love to complain about [legacy code](https://hachyderm.io/@norootcause/112012241401711355). However, there's a lot of truth to the concept. Old code never gets maintained as much as we'd like, and projects change goals and needs over time. When do you decide to rewrite parts of your code base? When do you throw them away entirely and start over? When do you dump frameworks in favor of newer techs? Would you ever swap out databases with multiple millions of rows?

## Type checking in 2025

Most type-checking these days has begun and ended with "use mypy." Mypy is great, but given Microsoft's abundance of VS Code and pylance/pyright built-in, is it time to revisit that assumption? Are there other options that work well with Django out there?

## Security

Yeah, this is an extremely broad concept and has lots of layers involved, but how do you protect yourself from malicious actors? Whether it be more mundane stuff like DDoSes, credit card fraud, or script kiddies throwing things against the wall and seeing what sticks to more advanced adversaries, there's a lot out there that needs your attention.

## Database tips and tricks

There's a lot you can do here:

- Query optimization (within the ORM)
  - How to structure your ORM queries for better performance
  - How to structure your ORM queries for better readability
  - Using multiple read replicas for speed
- Deep dive into table configurations
- Getting started with a GIS project
- Much more!

## The Django, Python, and web dev communities: the past, the future, the present, the culture, the why, the who, and the what that makes it all possible

A lot of local communities are having trouble getting restarted in a post-acute-pandemic world. How do we rebuild local communities from almost nothing? How do we get people to step up and volunteer?

### Related: adapting communities to changes in life

The same communities we had before COVID can't be the same as they were before. People are 5 years older, and almost all of them have had significant life changes, whether marriages, divorces, children, or many other things, and it makes planning events much harder. How do you try to maintain some sense of community while adapting to these strange times?

## Using Django in machine learning projects

I'm not talking about "slap an LLM in there and call it a day." I mean how do you really use ML algorithms to make your users' lives better with meaningful data analysis that doesn't accidentally end up being a shortcut to the wrong answer?

## Performance and scaling

Not every project is going to be "webscale" (scare quotes fully intentional), but how do you expand your project to handle a few hundred users at once? A few thousand? These are much more common than a few million users at once.

## Deployment at any size

From tiny hobby projects (e.g. `fly deploy`) to massive megaliths, how do you deal with making sure deployments are as seamless and rapid as possible? What new techs are out there that make things better? What's new with django-simple-deploy?

## Career development

This is a really difficult topic to get right. You have a group of developers ranging in experience from less than a year to 30+ years of experience, and we're all interested in the same web framework. How do you thread that needle of encouraging the newer devs to spread their proverbial wings while not sounding like "you must follow this path to succeed"? Even worse, how do you avoid sounding like you're just dropping a bunch of buzzwords? You really have to know your audience well.

## Ethics in programming: all code we write has consequences and potential misuse

How can people use your code for evil? How can you prevent that? Should you? This one will not necessarily be Django-specific, but it's still an important topic

### GPTs, LLMs, and AIs, oh my!

How can you use generative models responsibly? Even if you can, should you? It's no secret that I look at technologies like GPT-x with deep suspicion, especially regarding the training sets used and the impact on climate required by such large amounts of computing power.

There are a few possible tracks I could see here:

- Can you justify using that much cloud computing in a climate crisis?
- Can you be sure that using such models won't open you up to potential copyright lawsuits?
- Can you be sure that using such models won't lead to embarassing results, like [racially diverse Nazis](https://www.theverge.com/2024/2/21/24079371/google-ai-gemini-generative-inaccurate-historical), which while well-intentioned, shows how even big players can get things horribly wrong?
- Can you get your project to be more than either a glorified party trick that gets obvious details very wrong[1] or a form letter generator?

[1] An important feature of charcoal grills is that they keep the fire [inside the grill](https://www.bing.com/images/create/a-chef-standing-on-the-edge-of-a-volcano-cooking-a/1-65e1dbf886c845ea92f4018d53a94880?id=DtAxxKK0NZu2dCkz5R6dSw%3d%3d&view=detailv2&idpp=genimg&idpclose=1&thId=OIG3.B4QPksiUZHE7pmAFL0Dl&frame=sydedg&FORM=SYDBIC), DALL-E.

## Personal growth: how the community helped you in some way and you'd like to pay it forward

This is one that really hits close to me, especially after my own story of loss (that's a heavy one and I'm still not sure I'm ready to share it without breaking down 10 years later), but the Django community is really great and did a lot for me personally to help me both in my career and also in meeting new lifelong friends.

If you have any sort of story you'd like to share, this would be a great platform for it.

## Something else entirely?

Do you have an idea for a talk that's so out of left field that it doesn't fit anywhere in here? What the hell, submit it anyway! The worst thing that could happen is that we say no!
