---
title: Create a Blog Post
sidebar_position: 3
slug: /create-a-blog-post
---



# Create a Blog Post {#d5a52d2b2528488c952821b0d4b7ce53}


Docusaurus creates a **page for each blog post**, but also a **blog index page**, a **tag system**, an **RSS** feed…


## Create your first Post {#7d58ff713af1464c8e3f9012cc9d270e}


Create a file at `blog/2021-02-28-greetings.md`:


```markdown
---
slug: greetings
title: Greetings!
authors:
	- name: Joel Marcey
		title: Co-creator of Docusaurus 1
		url: https://github.com/JoelMarcey
		image_url: https://github.com/JoelMarcey.png
	- name: Sébastien Lorber
		title: Docusaurus maintainer
		url: https://sebastienlorber.com
		image_url: https://github.com/slorber.png
		tags: [greetings]
---

Congratulations, you have made your first post!

Feel free to play around and edit this post as much as you like.
```


A new blog post is now available at [http://localhost:3000/blog/greetings](http://localhost:3000/blog/greetings).

