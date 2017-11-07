# Python
Study Python Recording and Some notes here!

## Change Ancount in Tortoisegit
* what

I have logined [Coding]('https://coding.net/') ancount in TortoiseGit. Now I want to change the ancount and login [Git](https://github.com/) ancount to using it.

————————————————
* How

It seems that don't need to change ancount in setting, jsut 'clone' a project from Git and then pull changed file!

Now I have changed the README.md, I must commit it to local repository!Successfully in test commit!

Notice that **commit** operation just commit change in **local repository**, but I want to I can see the change online, I need to pull project!

————————————————

**Pull project** operation will uploading the project change to online!

when pull project, Tortoisegit give window to login GitHub, enter correct username and password everything is ok!

Now I have knew how to commit and pull my project to GitHub, I will try my best to use it!

Good luck!

***
## Incremental store data
When using Scrapy crawl data from html, I usually find the html, contained data I need, will update! When it happend I start my spider to crawl, but I just need to crawl the updated htmls to save time and space!

So, I need to determine:
1. which urls are new --- judge url in mysql or not
2. How to call spider correctly --- use if statement
3. How to save these data --- insert into mysql

Firstly, I try to judge urls in *spider.py* which in my scrapy project! And it works well!

But I think there maybe have better ways to solove this problem, So I try to use middlewares. In scrapy, there have Downloader middlewares and Spider Middlewares. I try filtering urls in *spider middlewares*, the testing print code works well but it can't filter urls! When I filtered urls in parse function of spider.py, it works well!
