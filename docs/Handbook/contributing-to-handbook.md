---
title: Contributing to the Handbook
sidebar_position: 1
slug: /contributing-to-handbook
---



# Contributing to the Handbook {#4cbbb6f7416a43a3a495a7011abc4cc5}


Two major steps are needed to contribute to the handbook:

1. Create the document(s) on Notion.
2. Use GitHub Action to publish the document.

## Create the Document on Notion {#db5590b13da042b18c7728c426370f74}

1. **Navigate to the** [**Handbook Database**](https://www.notion.so/3dc8e0950bb7445b876d2b179a44ff1d)  **page**

	All documents in the handbook are created from this database. Ensure you create a status ID for your document if it doesn’t belong to any existing ID.


	![](/notion_imgs/624321491.png)

2. **Create status ID**

	A status ID is required to publish only the documents you wish to publish on the website at that time. To create one:

	1. Hover over the database and a toolbar will appear.

		![](/notion_imgs/64511270.png)

	2. Click the horizontal ellipsis icon (three dots).

		![](/notion_imgs/1456831778.png)

	3. Click _**Properties**_ from the action panel.

		![](/notion_imgs/1762392665.png)

	4. Click on **Status**.

		![](/notion_imgs/1552177403.png)

	5. Click on the **`+`** icon opposite the **Options** text.

		![](/notion_imgs/172845811.png)

	6. Enter a unique status name.
3. **Add new document**
	1. Return to the **Database** section.
	2. Click on the **New** button.

		![](/notion_imgs/470757847.png)

	3. Enter the document title.
	4. Choose a **Category**.
	5. Choose the **Status** you added.
	6. Add slug (path name for the document) e.g., if your document is titled **General Onboarding**, the corresponding slug should be `/general-onboarding`.
	7. Add the contents of your document.

		:::caution
		
		Docu-notion is a tool that downloads Notion documents and converts them to markdown. However, it's important to note that not all blocks are supported by Docu-notion. For example, multi-column blocks are not supported.  You can review this **[Problem Internal Link]** to see what each block would look like when the document is published.
		
		:::
		
		

4. **Add document links to the Outline page**

	After creating your documents, you need to add links to them on the **[Problem Internal Link]** page. This ensures they appear in the correct order on the website's sidebar navigation when published. Follow these steps:

	1. Navigate to the **Outline** page.

		![](/notion_imgs/331298246.png)

	2. Locate the appropriate category page for your document and click the page link.
	3. If your documents are to be placed under a subcategory:
		1. Create a new page within the category page.
		2. Give the new page a title.
	4. Add the document link:
		1. Copy the URL of the document.
		2. Click on the category or subcategory where you want to add the link.
		3. Paste the URL and select **Link to Page**.

			![](/notion_imgs/790611638.png)

	5. Repeat steps 4a-4d for each document you want to add.
	6. Arrange the links in the desired order within their category or subcategory.

		:::tip
		
		The order of links on the **Outline** page determines the order in which documents appear in the sidebar navigation on the published website.
		
		:::
		
		


# Publishing Documents Using GitHub Action {#f179b90a0f7b4bbfa3149cbe26490f11}


After creating and obtaining approval for your Notion documents, follow these steps to publish them:

1. Go to the [handbook repository](https://github.com/Projectstake/docu-notion-sample).
2. Create an issue and a new branch:
	1. Click the **Issues** tab.

		![](/notion_imgs/1045437266.png)

	2. Create a new issue.

		![](/notion_imgs/1974701907.png)

	3. Create a branch from this issue.

		![](/notion_imgs/1478619668.png)

3. Run the document download workflow:
	1. Navigate to the **Actions** tab.

		![](/notion_imgs/1383545313.png)

	2. Click **Download and Commit Notion Docs**.

		![](/notion_imgs/402052963.png)

	3. Click the **Run workflow** dropdown, select the new branch, enter the **Status Tag** name, and enter a commit message.

		![](/notion_imgs/271666376.png)

	4. Click **Run workflow**.

		![](/notion_imgs/1533920620.png)


		This action pulls all documents tagged with the specified status into your new branch.

4. Create a pull request:
	1. Go to the **Code** tab.
	2. From the branch dropdown (labeled **main** by default), select your new feature branch.
	3. Click **Contribute**, then **Open pull request**.

		![](/notion_imgs/954939981.png)


		A GitHub Action will run automatically to create the pull request.

5. Review and approve the changes:
	1. Navigate to the **Pull Requests** tab.
	2. Open the newly created pull request.
	3. Wait for the preview link to appear in the comments.

		![](/notion_imgs/1595425803.png)

	4. Click the link to verify that your document renders correctly on the website.
	5. Confirm that the pull request passes all relevant tests.
	6. Request a review.

Once approved, the maintainer will rebase and merge your pull request into the main branch.

