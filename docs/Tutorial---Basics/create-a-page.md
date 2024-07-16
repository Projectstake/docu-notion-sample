---
title: Create a Page
sidebar_position: 2
slug: /create-a-page
---



# Create a Page {#1e0442b11f6446bab668b86d6123b4a2}


Add **Markdown or React** files to `src/pages` to create a **standalone page**:

- `src/pages/index.js` → `localhost:3000/`
- `src/pages/foo.md` → `localhost:3000/foo`
- `src/pages/foo/bar.js` → `localhost:3000/foo/bar`

## Create your first React Page {#7b9aa0de43bf48d1bdbaf2e962e5837d}


```javascript
import React from 'react';
import Layout from '@theme/Layout';

export default function MyReactPage() {
  return (
    <Layout>
      <h1>My React page</h1>
      <p>This is a React page</p>
    </Layout>
  );
}
```


A new page is now available at [http://localhost:3000/my-react-page](http://localhost:3000/my-react-page).


## Create your first Markdown Page {#9ce0109dd730425f8a477e462af4a263}


Create a file at `src/pages/my-markdown-page.md`:


```markdown
# My Markdown page

This is a Markdown page
```


A new page is now available at [http://localhost:3000/my-markdown-page](http://localhost:3000/my-markdown-page).

