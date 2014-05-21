The Creed of Software Engineering
=================================
by: Daft Labs

in no particular order:

- names matter
  - branding 
    - brand names and domain names should match
    - names should:
      - be easy to pronounce
      - be real words
      - contain as few syllables as possible
      - have no missing or replaced letters
      - not sound like other words (ex: daft gets confused with deft regularly)
  - programming
    - don't abbreviate
    - when the meaning of an element (variable/method/class) changes, change the name (but srsly, put serious thought into the names)
    - Be consistent.

- less cogs in the machine with the same level of functionality should be the goal
  - keep complexity as low as possible
  - celebrate deletions, not addtions
  - http://blog.newrelic.com/2013/05/02/red-code-green-code/

- programming
  - http://en.wikipedia.org/wiki/Rubber_duck_debugging
  - languages can be messy. you can do a lot of things a lot of different ways. have a convention
    - php: http://pear.php.net/manual/en/standards.php
    - Be consistent.
    - line length should be less than 100 characters (github's panel width)
    - clarity of code and readability are more imprtant than basically everything else
    - frameworks have conventions
      - don't roll your own
  - don't get defensive when talking about the product. (ex: don't shy away from things you know are hard)
  - have tests
    - run your tests
      - frequently
  - all code should be pull requested, all members of the team should read pull requests and give some quorum of :cake: or :princess:
    - tests should be run against every pull request automatically
  - markup and css belong in templates, not controllers or models
  - don't have credentials under version control
  - don't commit dependency code (i.e. jquery, bootstrap)
    - use composer or npm or gems or submodules or anything
  - don't roll your own framework
    - bootstrap for markup and chrome
    - jquery for javascript
    - angular for interactions
    - laravel for php
    - express for nodejs
    - rails for ruby
    - django for python
  - evaluate performance when it becomes a business problem
    - seriously, don't prematurely optimize
      - no really, you aren't going to have a million users day one of launch. if you do, good for you. deal with it then.
  - globals are bad. mmmm'kay?

- two people working on a project, especially on the tech side, are infinitely better than one (http://feedfront.com/archives/article006974)
  - make your "bus number" as high as possible (http://en.wikipedia.org/wiki/Bus_factor)

- ideas are worth almost nothing; execution is worth everything (http://www.shoemoney.com/2014/05/05/find-technical-co-founder)

- ops
  - deployments should be atomic, as automatic as possilbe and happen often (https://github.com/blog/1241-deploying-at-github and http://codeascraft.com/2010/05/20/quantum-of-deployment)
  - setting up servers and development environments should be as quick and easy as possible (http://www.vagrantup.com/ and http://www.getchef.com/)
    - the amount of information in your head, not represented in code, should be as small as possible
    - development and production should be as similar as possible
    - as soon as you have one system level dependency for your project, you should be using a virtual machine (vagrant).
- don't hire anyone that can't use git from the command line or isn't willing to learn (http://nfarina.com/post/9868516270/git-is-simpler)
- project management and communication are very important
  - programmers define difficulty
  - business defines goals
  - product defines priority
  - nobody bitches. we're a team.
  - time doesn't matter. results matter
    - the number of hours worked is not a representation of productivity
  - sleep is important (majestic if you will)

- Basically anything here: http://pivotallabs.com/category/tech-talks
  - but specifically this: http://pivotallabs.com/103-agile-the-pivotal-way/

- programming sucks. --> http://stilldrinking.org/programming-sucks

- use the right tool for the job. don't try to fit a square peg in a round hole. (ex: don't do caching in mysql. this is why we have memcached).

- don't use caching until absolutely necessary. it's for scale, not a bandaid for terribly optimized apps.

- use math, not feelings. that doesn't mean you can't use feelings sometimes, but you have to admit it.
  - Be consistent.

- know the value of your resources
  - sometimes it's cheaper to have a human do the job instead of writing a program (ex: modify these 10 records)
  - if a server is messed up, and it's not a recurring problem, since you use chef, you can just nuke it and make a new one. don't try to fix the problem.
  - work on high value, low cost features first.

- product
  - design isn't nearly as important as function. build out your features before adding chrome. UX people first, programmers second, designers third.
  - know where you're going, but build your MVP first. (don't build an oil tanker when you need a tugboat)
  - MVP should be the smallest possible (not completely useless) piece of the great whole
    - bulid for what you need now, not what you expect you might need in the future
  - pages should have only one call to action
  - Be consistent.
- team dynamic is important. bolster the 'family' feeling by doing unstructured extra-curricular activities
  - farmhouse thursdays
  - bierhaus thursdays
  - thirsty thursdays
  - burger wednesdays
  - team lunch (no fucking working)

- http://highscalability.com/

- pirates code applies here (https://www.youtube.com/watch?v=b6kgS_AwuH0)
