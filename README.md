The Creed of Software Engineering
=================================
by: Daft Labs

in no particular order:

- [focus](http://www.commitstrip.com/wp-content/uploads/2014/11/Strip-Side-project-650-finalenglish.jpg)
- [ideal stack](http://stackexchange.com/performance)
- [configurations](https://github.com/jtgraphic/configurations)
- learning? [great advice] (https://np.reddit.com/r/learnprogramming/comments/2qznse/i_need_serious_help_learn_to_program_was_my_new/cnb1luk)
- math not feelings
  - [Ad spend calculator](http://ad-spend-calculator.qwilr.com/)
- names matter
  - branding 
    - brand names and domain names should match
    - names should:
      - be easy to pronounce
      - be real words
      - contain as few syllables as possible
      - have no missing or replaced letters
      - not sound like other words (ex: daft gets confused with deft regularly)
      - the goal is to not have to explain or spell the name every time you tell it to someone.
      - names aren't as important as the brands you build them to be.
      - [generators](http://www.producthunt.com/jackdweck/collections/domain-discovery)
  - programming
    - don't abbreviate
    - when the meaning of an element (variable/method/class) changes, change the name (but srsly, put serious thought into the names)
    - Be consistent.

- less cogs in the machine with the same level of functionality should be the goal
  - this conflicts with the idea of "using the best tool for the job", both are important you'll just have to figure it out on a case by case basis.
  - keep complexity as low as possible
  - celebrate deletions, not additions
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
    - don't comment out code. this is why we have version control.
    - your code should be clean enough to read without comments.
      - comments are okay in rare occasions like heavy math, but ultimately are out of date as soon as you write them.
    - if you're unsure about syntax, test it! Use a [REPL](https://repl.it)
  - don't get defensive when talking about the product. (ex: don't shy away from things you know are hard)
  - have tests
    - run your tests
      - frequently
      - worst case scenario, [rainforest qa](https://www.rainforestqa.com/)
  - all code should be pull requested, all members of the team should read pull requests and give some quorum of :cake: or :princess:
    - tests should be run against every pull request automatically
    - blockers should be explicitly stated
  - markup and css belong in templates, not controllers or models
    - there are these things called templating languages, use one
      - php: [lavender](https://github.com/golavender/lavender) or [twig](http://twig.sensiolabs.org/)
      - node: [jade](http://jade-lang.com/)
  - don't have credentials under version control
  - don't commit dependency code (i.e. jquery, bootstrap)
    - use composer or npm or gems or submodules or anything
  - don't commit "built" files like compiled sass, etc.
  - don't roll your own framework
    - bootstrap for markup and chrome
    - jquery for javascript dom management
    - lodash for more javascript helpers (this has some overlap with jquery, use jquery for dealing with jquery objects and lodash for everything else)
    - angular for javascript interactions (lets you build most of your ui javascript interactions directly into the markup instead of having one off scripts for stupid things. beware of large data sets)
    - laravel for php
    - express for nodejs
    - rails for ruby
    - django for python
  - evaluate performance when it becomes a business problem
    - seriously, don't prematurely optimize
      - no really, you aren't going to have a million users day one of launch. if you do, good for you. deal with it then.
  - globals are bad. mmmm'kay?
  - form posts ALWAYS redirect. dont just process the post and render something on the same request
  - know a little bit about security
    - security audits will get the crazy stuff, but you should know the basics
    - [interesting post about password cracking](https://community.qualys.com/blogs/securitylabs/2012/06/08/lessons-learned-from-cracking-2-million-linkedin-passwords)
    - [key stretching](http://en.wikipedia.org/wiki/Key_stretching)
    - [do we even need passwords?](https://medium.com/cyber-security/9ed56d483eb)
  - [keep your bedroom clean](http://www.commitstrip.com/en/page/6/)
    - commit (pun intended) a meaningful amount of time to optimizing and cleaning your code.
    - pay technical debt as soon as possible.
    - some times it's just too messy. the sign of a great leader is someone that is willing to [throw away all of their code.](http://www.commitstrip.com/en/page/21/)
      - [don't go overboard though](http://www.commitstrip.com/en/page/50/)

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
  - [time doesn't matter. results matter](http://www.commitstrip.com/en/page/35/)
    - the number of hours worked is not a representation of productivity
  - sleep is important (majestic if you will)
  - invest in tools that save time
    - [hub](https://github.com/github/hub)

- Basically anything here: http://pivotallabs.com/category/tech-talks
  - but specifically this: http://pivotallabs.com/103-agile-the-pivotal-way/

- all programming languages are broken. [watman](https://www.destroyallsoftware.com/talks/wat)
- [programming sucks](http://stilldrinking.org/programming-sucks)

- use the right tool for the job. don't try to fit a square peg in a round hole. (ex: don't do caching in mysql. this is why we have memcached).

- don't use caching until absolutely necessary. it's for scale, not a bandaid for terribly optimized apps.

- use math, not feelings. that doesn't mean you can't use feelings sometimes, but you have to admit it.
  - Be consistent.

- know the value of your resources
  - sometimes it's cheaper to have a human do the job instead of writing a program (ex: modify these 10 records)
  - if a server is messed up, and it's not a recurring problem, since you use chef, you can just nuke it and make a new one. don't try to fix the problem.
  - http://en.wikipedia.org/wiki/Peter_Principle - promoting from within isn't always a good idea
  - work on high value, low cost features first.

- product
  - [UX Checklist](http://uxchecklist.github.io/)
  - functionality is more important than design. build out your features before adding chrome. UX people first, programmers second, designers third.
  - know where you're going, but build your MVP first. (don't build an oil tanker when you need a tugboat)
  - MVP should be the smallest possible (not completely useless) piece of the great whole
    - build for what you need now, not what you expect you might need in the future
  - pages should have only one call to action
  - be vocal about things you think are broken or inefficient
  - Be consistent.
- team dynamic is important. bolster the 'family' feeling by doing unstructured extra-curricular activities
  - farmhouse thursdays
  - bierhaus thursdays
  - thirsty thursdays
  - burger wednesdays
  - team lunch (no fucking working)
  - know your programmer humor
    - [commit strip](http://www.commitstrip.com/en/)
    - [xkcd](http://xkcd.com/)
    - [reddit: programmer humor](http://www.reddit.com/r/programmerhumor)
  - make sure everyone is aware of the [cost of meetings](http://tobytripp.github.io/meeting-ticker/)

- http://highscalability.com/
- https://www.destroyallsoftware.com/talks

- invest in equipment that increases efficiency, but don't invest in things that satisfy your ego.
  - [whitepaper on screen size vs. productivity](http://pfeifferreport.com/Cin_Disp30_Bench_Rep.pdf)
- [pivotal and git integration](http://pivotallabs.com/level-up-your-development-workflow-with-github-pivotal-tracker/)
- [you can't make everyone happy](http://xkcd.com/1172/)

- [and most importantly](https://www.youtube.com/watch?v=b6kgS_AwuH0)
  - [penalties](http://www.commitstrip.com/en/page/42/)
