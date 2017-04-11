Daft Labs Software Engineering Creed
====================================

### "Math Not Feelings"

March 2017

# On Culture
* Frequent team lunches, no shop talk
* Understand the [cost of meetings](http://tobytripp.github.io/meeting-ticker/)
* [Every change breaks someone’s workflow](https://xkcd.com/1172/)
* Humor
    * [commit strip](http://www.commitstrip.com/en/)
    * [xkcd](http://xkcd.com/)
    * [reddit: programmer humor](http://www.reddit.com/r/programmerhumor)
# On Repositories
* Don’t commit:
    * Credentials
    * Commented-out code
    * Compiled Files
    * Dependency code (jquery, bootstrap)
        * Use composer, npm, gems, bower or any other dependency management system.
* Line length should be <= 100 characters (github’s diff panel width).
* Commits should be present tense
    * "Fixing the bug" vs “Fixed the bug”
# On Design
* Functionality is more important than design.  Build out features before adding chrome.  User Experience Design > Programming > High-Res Design
* Understand your end goal, build your minimum viable product first.  Don’t build an oil tanker when you need a tugboat.
    * The goal of an MVP is to build the smallest possible piece of the whole that will enable you to test market viability > reflect > iterate.  Build what you/consumers need now, not what you expect you might need in the future.
* Each marketing page should have a call-to-action.  An effective page has as few calls-to-action as possible.
* Sometimes it’s cheaper to have a human do the job
# On Project Planning
* Programmers define difficulty > Business defines goals > Management defines priority
* Keep complexity as low as possible
* **Keep a Low Bus Factor** - the [Bus Factor](https://en.wikipedia.org/wiki/Bus_factor) is a measurement of risk resulting from information and capabilities not being shared among team members.  Information should be fluid as possible, avoid creating key irreplaceable members.  What would happen if they were to be hit by a bus and disappear from the project?
    * Zero is idealistic
    * Otherwise, aim for high bus factor - # of people who can disappear before project fails
* **Avoid Premature Optimization** - are you going to have a million users on day one?  If not, scalability should be deprioritized.  Evaluate performance when it becomes a business problem.
# On Development Cycles
* Pay technical debt as soon as possible.
* High value, low cost features first.
* [Brooks’s Law](https://en.wikipedia.org/wiki/Brooks%27s_law), "adding manpower to a late software project makes it later"
    * **Plan Ahead** - it takes time for people added to a project to become production due to ‘ramp up time.’
    * **Keep Teams Lean** - communication overhead increases as the number of people increases due to the need to keep in sync.
    * **Cooks in the Kitchen** - is the project divisible by an additional member?  "It takes one woman nine months to make a baby, but nine women can’t make a baby in one month."
    * **Exceptions**:
        * Projects can be brought back into (or kept in) control if people are added earlier in the process.
        * The law can be circumvented by overrunning a project in such a way that extra capacity compensates ‘ramp up time’ and communication overhead.
# On Development
* Results matter, delivery is key
    * Number of hours worked is a representation of productivity, not value
    * [Avoid the temptation of shiny new projects/frameworks](http://www.commitstrip.com/wp-content/uploads/2014/11/Strip-Side-project-650-finalenglish.jpg)
* Problem solving techniques
    * **Rubber Duck Debugging** - Many find in explaining a problem to someone that they hit upon a solution.  To avoid interrupting anyone, instead teach an inanimate object how to go about something, or explain the problem to it line-by-line.  This allows you to evaluate your thoughts from different perspectives.
    * **Break the Problem Down** - [great article](https://np.reddit.com/r/learnprogramming/comments/2qznse/i_need_serious_help_learn_to_program_was_my_new/cnb1luk/).
* Balance
    * [Sleep is so important](https://www.bustle.com/articles/140910-what-happens-to-your-body-when-you-dont-sleep)
    * Celebrate deletions not additions, but to a point.  Understand what [red code](https://blog.newrelic.com/2013/05/02/red-code-green-code/) is.  Clarity of code and readability is more important than anything else.
    * Your code should be clean enough to read without comments.  Comments are okay in rare occasions like heavy math, but should be avoided.
    * Invest in tools that save time, but avoid stroking ego
        * [Github hub](https://github.com/github/hub)
        * [Productivity vs Screen-Size](http://pfeifferreport.com/Cin_Disp30_Bench_Rep.pdf)
* Consistency
    * [Syntax](https://repl.it/)
    * Language conventions
        * [PHP](http://www.php-fig.org/psr/psr-2/)
        * [HTML/CSS](https://google.github.io/styleguide/htmlcssguide.html)
        * [Javascript](https://google.github.io/styleguide/javascriptguide.xml)
    * Frameworks have conventions, don’t roll your own
    * Markup/CSS belongs in templates, not controllers or models
        * Use templating languages
            * PHP
                * [Lavender](http://golavender.com)
                * [Twig](http://twig.sensiolabs.org/)
            * Node
                * Pug ([Jade](https://github.com/pugjs/pug))
# On Stacks
* Bootstrap - markup and chrome
* Lodash - js object/array helper suite
* React - dom management
* Redux - state management
* Laravel - php framework
* Genesis - wordpress theme framework
* Jekyll - static sites
* Rails - ruby framework
* Django - python framework
# On Security
* Know the basics
    * [Password cracking](https://blog.qualys.com/securitylabs/2012/06/08/lessons-learned-from-cracking-2-million-linkedin-passwords)
    * [Key stretching](https://www.wikiwand.com/en/Key_stretching)
    * [Do we need passwords?](https://medium.com/@ninjudd/passwords-are-obsolete-9ed56d483eb#.5bpme0u45)
# On Advertising
* Should I pay for advertising?
    * We recommend using this [ad spend calculator](http://ad-spend-calculator.qwilr.com/).  Calculating the Life Time Value (LVT) of a customer is the first step in determining your paid advertising budget.
# On Branding
* Where should I begin when creating my brand name?
    * We recommend using a [domain discovery tool](https://www.producthunt.com/@jackdweck/collections/domain-discovery).  Brand name and domain should match to help consumers and search engines find you.  A domain will be a key asset to your business so start here.
* What constitutes an effective brand name?
    * Easy to pronounce, easy to spell
    * A combination of recognizable (not-made-up) words
    * As few syllables as possible
    * Avoid missing or replace letters
    * Make it a goal to not have to explain or spell the name every time you tell someone
