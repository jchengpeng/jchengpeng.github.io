---
layout: post
title:  "My first blog in github!"
date:   2018-07-04 09:24:32
categories: java
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight java %}
       
        if (StringUtils.equals(flag, "1")) {

            PageList pageList = (PageList) purchase;

            int totalPages = pageList.getPaginator().getTotalPages();

            result.put("totalPages", totalPages);

            result.put("list", purchase);

            return generateResponse(result);
        }
#=> the example for java.
{% endhighlight %}
