fCMS

The goal was to create a simple CMS, minimizing the features that I do not
want, and keeping page-load times as low as possible.

The initial impetus was seeing yet another wordpress site violated by robots
and seeing page load times creep into the 10s of seconds for useless content
to load alongside or even before the content you actually wanted to see.

The code isn't pretty, I can't guarantee it will do anything you want it do.

But I have been running it in place of wordpress and quite happy with it,
adding tiny features here and there.

Bear in mind, this is a VERY spartan "CMS", if you can even call it that.

A better description would be database reader that happens output to web
paired with a database injector that does not take input from web.

In order to make a "post", you must be able to edit post.txt in the directory
where post.py exists.  You must then run post.py with permissions to modify
the database (./html/db/content.db).  Basically you've gotta buck up and do
some old-school sysadmin stuff to update your page, but that's cool... and I
will explain why.

Firstly, it's easier to keep an eye on what is happening with your webserver
if you are not running an overly complicated stack.

Secondly, unless you actually have a need for an overly complicated stack,
why have it?

Lastly, if you're like me and really just keep a blog for the fun of it,
perhaps you're tired of constantly having to do system updates for both the
OS and the CMS.

That last one bears a bit more explanation.  I'm not saying that you can
stop doing updates, what I'm saying is by running a simple, transparent code
base that you can read through and see what it does, you are empowering
yourself.  Bigger, more feature-rich CMS's are great, they're just too big 
for smaller sites, and not a great starting point for understanding how a 
"website" works.

Including this README, fCMS is literally five files and two directories.

total 16K
1.6K Aug 24 16:48 post.py
944b Aug 24 16:48 post.txt
886b Aug 24 16:52 README.md

./html:
total 8.0K
2.1K Aug 24 16:48 index.php

./html/db:
total 8.0K
8.0K Aug 24 16:48 content.db

I've been using this with nginx for some time, but it should work equally well
on any webserver that supports PHP, python, and sqlite.

If someone else already uses the name fCMS, I am sorry, please don't sue.
This is a FOSS project and I don't make enough money for a lawsuit to make
sense anyway.  I chose f for Femto: 
Femto- (symbol f) is a unit prefix in the metric system denoting a factor of 10−15

