---
layout: post
title:  "Welcome to Jekyll!"
date:   2023-09-18 09:00:49 +0200
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight sql linenos %}
-- This is a comment
select 42
from   dual;
{% endhighlight %}

{% highlight sql linenos %}
-- This is a comment
create table t (
  x int  primary key generated always as identity,
  y text not null check (y <> '' and y <> 'my big no-no string')
);

-- This is a comment
create function f(x int)
returns real as $$
  select sum(t.y + (select 42 from dual)) + f.x
  from   t
  where  t.y <> 42;
$$ language sql;
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
