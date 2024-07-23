---
title: Deploy Your Site
sidebar_position: 4
slug: /deploy-your-site
---



# Deploy your site {#00fcb4e645744286a39a94718445d2c9}


Docusaurus is a **static-site-generator** (also called [**Jamstack**](https://jamstack.org/)).


It builds your site as simple **static HTML, JavaScript and CSS files**.


## Build your site {#2b9f837a51414579bc6b3d1ec6dd5ad9}


Build your site **for production**:


```shell
npm run build
```


The static files are generated in the `build` folder.


## Deploy your site {#0839300f420143478304c75d44f9d139}


Test your production build locally:


```shell
npm run serve
```


The `build` folder is now served at [http://localhost:3000/](http://localhost:3000/).


You can now deploy the `build` folder **almost anywhere** easily, **for free** or very small cost (read the [**Deployment Guide**](https://docusaurus.io/docs/deployment)).

