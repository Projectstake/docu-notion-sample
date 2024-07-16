---
title: Create a Document
sidebar_position: 1
slug: /create-a-document
---



# Create a Document {#504d31940b3a4c1caf0153033bab3320}


Documents are **groups of pages** connected through:

- a **sidebar**
- **previous/next navigation**
- **versioning**

## Create your first Doc {#495da6f726604f658b6725e0bcde561f}


Create a Markdown file at `docs/hello.md`:


```markdown
# Hello

This is my **first Docusaurus document**!
```


A new document is now available at [http://localhost:3000/docs/hello](http://localhost:3000/docs/hello).


## Configure the Sidebar {#6a3364928e834605afb5c40da5b2d6c5}


Docusaurus automatically **creates a sidebar** from the `docs` folder.

Add metadata to customize the sidebar label and position:


```markdown
---
sidebar_label: 'Hi!'
sidebar_position: 3
---

# Hello

This is my **first Docusaurus document**!
```


It is also possible to create your sidebar explicitly in `sidebars.js`:


```javascript
export default {
  tutorialSidebar: [
    "intro",
    // highlight-next-line
    "hello",
    {
      type: "category",
      label: "Tutorial",
      items: ["tutorial-basics/create-a-document"],
    },
  ],
};
```

