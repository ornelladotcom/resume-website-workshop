# Adding style to a page

As you've seen, [HTML is used to structure the content](./2-add-content.md) of a page. CSS, or Cascading Stylesheets, is used to provide style. CSS is used to set colors and fonts, where on a page information should be displayed, and other decorative items. By keeping HTML and CSS focused on these concerns (sometimes called separation of concerns), you create pages which are easier to modify and maintain, and become more accessible to all users.

## Introducing selectors

CSS uses **selectors** to indicate what to modify. These selectors can be the name of a tag such as `h1`, an attribute such as `class` or `id` - useful for modifying a group of elements or one specific one respectively, or get really fancy and look at the entire structure of a page to determine what to modify. We're going to focus on using tag names as selectors.

When using a tag name for a selector, you use just the name of the tag. Keep in mind, when you indicate the name of a tag, the style applies to **all** tags.

> **Note:** The word "cascading" for Cascading Stylesheets applies when multiple styles are used for the same element.

## Adding style to a page

Let's start by adding style to the page. We'll set a couple of properties for the `body` tag to change the font and size.

1. Return to Visual Studio Code
1. Inside **style.css**, add the following CSS to choose the font and size

    ```css
    body {
        font-family:Arial, Helvetica, sans-serif;
        font-size: 14px;
    }
    ```

Notice `font-family`, which is used to select the font. There are three fonts listed. Because users may not have a particular font installed, CSS offers the ability to fallback to the next font. In this case you're telling the browser to try Arial first, then Helvetica if that's not installed, and finally any sans-serif font.

## Sizing

CSS offers different ways to indicate sizes. In the example above, you used `18px`. `px` stands for pixels, and is an absolute sizing - it will always be 18 pixels regardless of the screen used. The problem with using absolute sizing is modifications to the size require updates to multiple styles. By using relative sizing, you use a single base; updates to the base then update the rest of the page.

For our example we'll use `rem`. `rem` indicates the size of the font at the root element - `body` in our example. `rem` is a 1 based value, where `1rem` is the size of the root element, `1.5rem` is one and a half times the size, and `.25rem` is one quarter the size.

Let's set the size for our different header elements.

1. Return to Visual Studio Code
1. At the bottom of **style.css**, add the following to set the size for the `h1` - `h4` tags

    ```css
    h1 {
        font-size: 1.4em;
    }

    h2 {
        font-size: 1.2em;
    }

    h3 {
        font-size: 1.1em;
    }

    h4 {
        font-size: 1em;
    }
    ```

1. The page updates with the new sizes
1. Save all files by selecting **File** > **Save all**

## Summary and next steps

You have successfully added style to a page. You chose the font you wish to use, and set sizes for various elements. To complete your resume, you'll [control where elements are displayed](./4-location.md) on the page.
