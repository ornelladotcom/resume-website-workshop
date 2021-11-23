# Adding content to an HTML page

[Previously](./1-create-html.md) we saw how to create the structure of an HTML page. Now we want to begin adding content to our resume. Specifically, we want to add an email address, social media, education and experience.

## Creating email links

Let's start by creating a link to your email address and any social media you wish to share on your resume. You'll use the `a` tag, which stands for "anchor". `a` has one attribute named `href` (short for hypertext reference). `href` will contain the address you want the link to point to. When a user selects the link, they will be taken to the page. If you want to create a link to an email address, you will use `mailto:` in front of the address; this will open the user's email client.

1. Return to Visual Studio Code
1. Inside **index.html**, and below the comment which reads `<!-- email address -->`, add the following HTML to add a link to your email, replacing **your-email@example.com** with your email address:

    ```html
    <a href="mailto:your-email@example.com">your-email@example.com</a>
    ```

1. The page automatically updates with your email address

> **IMPORTANT** Whenever you add a link to a page you want to ensure the text which is displayed for the link (commonly referred to as link text) accurately describes the target of the link. Text like **here** or **click here** aren't accessible because they don't help the user understand the significance of the link. Using [good link text makes your pages accessible](https://docs.microsoft.com/learn/modules/web-development-101-accessibility/4-links-images) to all.

## Creating lists

Lists come in two varieties in HTML - ordered (with numbers or letters) and unordered (bullet points). `ol` is used to create an ordered list and `ul` is used to create an unordered list; `li` indicates each "list item" in a list. Let's use an unordered list to create a list of our social media accounts.

You can add as many (or as few) social media links as you like, modifying the text as appropriate. The example below uses GitHub, LinkedIn and Twitter. Notice how it is possible to nest one tag inside another to create the display you wish.

1. Return to Visual Studio Code
1. Inside **index.html**, below the comment which reads `<!-- social media -->`, add the following HTML to create the list:

    ```html
    <ul>
        <li><a href="https://github.com/your_handle>">GitHub</a></li>
        <li><a href="https://linkedin.com/in/your_handle>">LinkedIn</a></li>
        <li><a href="https://twitter.com/your_handle>">Twitter</a></li>
    </ul>
    ```

1. The page will update to display the list of social media accounts you add

## Finishing out our resume

Let's close the last section of the page with our education and experience. Just as before, you can update the information to keep it about you and your background.

1. Return to Visual Studio Code
1. Inside **index.html**, below the comment which reads `<!-- education -->`, add the following HTML for your education information:

    ```html
    <h3>School name</h3>
    <h4>Major</h4>
    <ul>
        <li>GPA: 4.0</li>
        <li>Years attended</li>
    </ul>
    ```

1. Below the comment which reads `<!-- experience -->`, add the following HTML for your experience:

    ```html
    <h3>Company name</h3>
    <h4>Title</h4>
    <h4>Dates</h4>
    <ul>
        <li>Cool accomplishment</li>
        <li>Cool accomplishment</li>
    </ul>

    <h3>Cool hackathon</h3>
    <h4>Project title</h4>
    <h4>Dates</h4>
    <ul>
        <li>Cool accomplishment</li>
        <li>Cool accomplishment</li>
    </ul>
    ```

1. The window updates with your new information
1. Save all the files by selecting **File** > **Save all**

## Summary and next steps

You've now added the information for your resume! You also explored some of the most common HTML tags. But you may notice the display of the page is a little plain. Let's see how we can use [CSS to style the page](./3-add-style.md).
