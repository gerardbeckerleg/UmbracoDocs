---
versionFrom: 8.0.0
---
# Displaying the Document Type Properties

You might have noticed that the content we've added to the homepage is not being displayed. We need to wire up the Data Type properties to the template.  

Let’s look at our template and identify where the content should be displayed.

![Where our Data Properties Content Should be Output](images/figure-17-where-our-data-fields-go-v8.png)

The top arrow in this image is the _Page Title_ and the bottom arrow is the _Body Text_, whereas the Footer is all the way at the bottom.

## Setting the Document Type Properties

To set the Document Type properties:

1. Go to **Settings**.
2. Select **Templates** in the **Templating** section, and open the **Homepage** template.
3. Scroll down to the `<!-- Jumbotron, w title -->` section (around line 45) and highlight the text `“Welcome - UmbracoTV”`.
    ![Preparing to replace the hardcoded text with an Umbraco Page Field](images/figure-18-replace-hardcoded-text-with-umbraco-page-field-v8.png)
4. Click **Insert** and select **Value**.
5. Select **pageTitle** field from the drop-down list.
    ![Umbraco Page Field](images/figure-19-umbraco-page-field-v8.png)
6. Click **Submit**.
7. Repeat the same process for the content in the `<div class="container">` tag (around line 55):
    1. Highlight the content as shown in the figure.
    ![Replacing the bodyText with the Umbraco Page Field](images/figure-20-replace-bodytext-with-page-field-v8.png)
    2. Click **Insert** and select **Value**.
    3. Select **bodyText** field from the drop-down list.
    4. Click **Submit**.
8. Repeat the same process for the content in the `<div class="container-fluid footer">` tag (around line 144):
    1. Highlight the content between the `<div class="container">` tags.
    ![Replacing the Footer Text with the relevant Umbraco Page Field](images/figure-21-footer-text-v8.png)
    2. Click **Insert** and select **Value**.
    3. Select **footerText** field from the drop-down list.
    4. Click **Submit**.
9. Click **Save**.

Reload your homepage to view the content. You should see something similar like the image below:
![Displaying the Document Type Properties](images/figure-22-displaying-document-type-properties.png)

Now, you can go back and add additional fields or update existing fields in the Document Type, fill them out in the content node and then add them in the template to display the data in the website.

---

Prev: [CSS and Images](../CSS-And-Images) &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; Next: [Creating Master Template Part 1](../Creating-Master-Template-Part-1)