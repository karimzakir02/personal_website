---
title: "This Website"
date: 2024-01-09T11:56:54-05:00
draft: false
---

### Why?

I have been meaning to start a personal website for a while to discuss any projects I have worked on or explore any ideas I found interesting. I never considered myself a writer, though, and didn't think I would have fun writing articles/blogs, since I did not really enjoy writing in school. It's not something that I hated - or even disliked - but it wasn't my favorite activity either. 

After procrasting on the idea for some time, I discovered [Mike Crittended&rsquo;s website](https://critter.blog/). His blog is fairly simple - a collection of short articles written about a variety of topics, ranging from engineering to lifestyle. I loved the style of his blog, since it was personal and authentic, helping me realize that I don't have to overthink my structure or decisions when writing. I could just be myself and write however I liked, as long as what I wrote was coherent, well-structured, and interesting to me. After all, this blog is not graded, and I don't have to follow any specific rules or be otherwise constrained. Sure, my writing style is probably not going to impress anyone (at least right now) or be all that different from another person's, but I do want to get better at writing and have fun while doing so.

As such, welcome to my website/blog! In the rest of this article, I will discuss how I made this website from a technical point of view, in case you find this kind of stuff interesting or want to setup your own website.

### How?

This website is built using [Hugo](https://gohugo.io/) - a versatile framework for writing static websites, such as this one. The reason why I picked Hugo, instead of something like Jekyll or Gridsome, is that it seemed more versatile but still simple to use, meaning I could get a website going fairly quickly.

The theme I picked is the [Digital Garden Theme](https://digital-garden-hugo-theme.vercel.app/). A huge thank you to the [maintainers](https://github.com/apvarun/digital-garden-hugo-theme/tree/main#contributing) of this theme! Since I wanted to make some changes, I have decided to use my own fork of the original repo and add it as a submodule to the [website&rsquo;s Git](https://github.com/karimzakir02/personal_website).

I host this website on GitHub pages, since it's free and I don't have to buy a separate domain with my name in it. I love a good deal!

When setting up GitHub pages, I ran into some trouble with the CSS. Specifically, the website was retrieving the CSS at an incorrect link; this is because the CSS was located at `domain.com/personal_website/css/main.css`, but the website was trying to find it at `domain.com/css/main.css`. If you are running into the same trouble with this theme, navigate to the `head.html` file located in the layouts directory. There, in the \<link\> tag, change the link to the stylesheet to `/<repo_name>/css/main.css`. Don't forget the slash before your repo's name, it's essential!

If you are thinking about starting a blog yourself, I suggest reading _[just starting a dang blog](https://critter.blog/2020/12/24/just-start-a-dang-blog-already/)_ and _[the benefits of shorter writing](https://critter.blog/2020/12/24/just-start-a-dang-blog-already/)_ by Mike Crittended. Those articles gave me the final nudge to start writing, so maybe they will nudge you too!

Feel free to ping me if you have any suggestions about the website or any questions about how I made it! zakirkarim02 AT gmail DOT com. 
