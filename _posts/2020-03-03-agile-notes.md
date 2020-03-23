---
toc: true
layout: post
description: My Precious Notes on Agile Software Development
categories: [markdown]
title: On Agile
---
# General
* a lot of people think Agile is mainly about project management, but the
  creators of Agile put equal if not greater emphasis on engineering as well.
* the software craftsmanship movement preserves the coupling between practices
  and culture by emphasizing that technical practices are important for agile to
  be successful.
* For any behavior change, people learn first by practicing, and then learn to
  relate their practices back to principles and values.
* Agile is about doing the most valuable thing at any given moment.
* _Produce running, tested, working, integrated software every two weeks, every week. Build your skills until you can create a new fully operational version every day, twice a day, multiple times a day._
* _Agile is a set of values and principles generalized from the practices of several similar methodologies. Agile does not define any particular practices; but it has no meaning without them. Agile is the abstract class. Practices are the implementation._
    * Bob Martin on twitter
* PBI: product backlog items


# Extreme Programming
* invented by Kent Beck
* prior to scrum
* [dzone](https://dzone.com/articles/scrum-and-xp)
    * scrum and xp
    * _This book shows readers how to use Scrum, and Agile software development process, to quickly and seamlessly implement XP in their shops while still producing actual software. Using Scrum in the Agile process can virtually eliminate all downtime during an XP implementation._

## 12 Practices
* The Planning Game
* Small Releases
* Metaphore
* Simple Design
* Testing
* Refactoring
* Pair Programming
* Collective Ownership
* Continuous Integration
* 40-Hour Workweek
* On-site Customer
* Coding Standards

## Code Smells
* <img src="http://borlandc.pek3b.qingstor.com/soft-skill/code-smells.png" width=75%>


# Scrum
<img src="http://borlandc.pek3b.qingstor.com/devops/scrum.png" width=65%>

## Terms
* burndown - how much work is remaining to be done 
* burnup - how much work has been completed
* DRE - defect removal efficiency
    * DRE is the percentage of bugs identified and corrected internally compared to the total bugs in the complete release life cycle.
* CSAT - customer satisfaction

## User Story Map
<img src="http://borlandc.pek3b.qingstor.com/devops/user-story-mapping-3.png" width=75%>

User story mapping is a technique developed by Jeff Patton during his long practice as an Agile product owner/scrum master. A story map received its name because it helps map out user stories and other backlog items visually. Items are arranged in two dimensions: The vertical one denotes priority, while the horizontal one represents steps a user takes to perform actions in the system (user journey).


# Code Review
* [dzone](https://dzone.com/articles/4-types-of-code-reviews-any-professional-developer)
    * 4 types of code review
    * suggests async by default
* [smartbear](https://smartbear.com/learn/code-review/guide-to-code-review-process/)
    * general
    * performance
    * security
    * documentation
    * testing
* [atlassian](https://www.atlassian.com/agile/software-development/code-reviews)
* [dev.to](https://dev.to/codemouse92/10-principles-of-a-good-code-review-2eg)
    * practical principles of code review
* [nyu](https://nyu-cds.github.io/effective-code-reviews/03-checklist/)
    * effective code review check list
* [sonar-go](https://github.com/SonarSource/sonar-go)
    * replaces community plugin since May 2018
* [awesome code review](https://github.com/joho/awesome-code-review)
* [jboss](https://www.jboss.org/dms/judcon/presentations/Boston2011/JUDConBoston2011_day1track2session6.pdf)
    * slides about git but has 2 pages on code review
* [tips, 8](https://kellysutton.com/2018/10/08/8-tips-for-great-code-reviews.html)
    * _Latency is Key_

## Goals
* goal
    * catch bug
    * share knowledge
    * increase readbility
    * increase communication
    * learn, mentorship
* non goal
    * i am smarter than you
    * i write better code
    * you suck!

## Best Practices
* self review by author him/her self
* patch size matters
    * 400 lines or less, otherwise breaks into smaller commits
* time matters
    * 60 minutes or less
* think of all scenarios
* golang: separate vendor commit and actual change

## What to Review
* logic error
* correct and full understanding of requirements
* design: easy to implement, easy to understand
    * ask questions, discuss them!
* test: is there unit test that can be added?
* style: does the code conform to existing style
    * var name
    * comments adequte
    * function complexity?
* unchecked return value
* are all input checked?

# User Story
* _User Story is a small (actually, the smallest) piece of work that represents some value to an end user and can be delivered during a sprint._
* template
    * “As a [persona], I [want to], [so that].”
* **Epics** are large work items broken down into a set of stories, and multiple epics comprise an **initiative.** 
* Epics are not testable, otherwise, user stories should be testable
    * with the exception of non-funcitonal stories
* INVEST
    * independent
    * negotiable
    * valuable
    * estimable
    * small
    * testable
* [atlassian](https://www.atlassian.com/agile/project-management/user-stories)
    * apparently Atlassian knows something about user stories
* [stormotion](https://stormotion.io/blog/how-to-write-a-good-user-story-with-examples-templates/)
    * nice introduction article


# Scaling Agile
* LeSS - large scale scrum
    * Sprint Planning, Sprint Review and Sprint Retrospective runs at the same time for all teams.


# Culture

## Team Culture
<img src="http://borlandc.pek3b.qingstor.com/devops/team-culture.jpeg" width=75%>

* by a guy from Windows NT team
* referenced by Dave Chaney [here](https://dave.cheney.net/2020/02/23/the-zen-of-go)


# Links
* [infoq](https://www.infoq.com/news/2018/06/developers-should-abandon-agile)
    * Ron Jeffries says developers should abandon Agile
    * Faux Agile, Dark Agile
* [ronjeffries](https://ronjeffries.com/articles/018-01ff/abandon-1/)
    * developers abandon Agile
* [the manifestor](http://agilemanifesto.org)
* [wikipedia](https://www.wikiwand.com/en/Agile_software_development)
* [cleancoder](http://blog.cleancoder.com/uncle-bob/2018/08/28/CraftsmanshipMovement.html)
    * agile vs manager
* [infoq](https://www.infoq.com/articles/scrum-multiple-teams-frameworks)
    * multiple teams scrum framework
* [refactoring 2nd ed](https://www.slideshare.net/jexp/refactoring-2nd-edition)
    * slides on refactoring 2nd edition
    * by one of the book reviewer
* [martin, 2018, aus](https://martinfowler.com/articles/agile-aus-2018.html)
    * the state of agile in 2018
    * a talk Martin Fowler given in Austrilia
    * summary:
        1. Get rid of the Agile Industrial Complex and the idea of imposing stuff on teams. Let teams work out the way they should work themselves.
        1. Raise the importance of technical excellence, and never forget that when writing software, the technology side is really vital
        1. and organize around products.
* [infoq, metrics](https://www.infoq.com/articles/metrics-agile-teams)
    * The Importance of Metrics to Agile Teams
    * _Firstly, the reporting found within common workflow management tools like Jira is not optimised to provide the level of reporting that many teams require for an effective SI programme._
