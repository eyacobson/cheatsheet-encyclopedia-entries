The `<title>` Element
=====================

The `<title>` element/tag is required in all valid HTML documents. Its functions
include:

-   Supplying a title to be displayed in the browser toolbar and for the purpose
    of labeling an individual tab

-   Supplying a default title for the bookmark of the web page

-   Supplying a title for search engine results

-   Impacting search engine algorithms -- a well-constructed title can have
    positive effects on search engine optimization (SEO) for your web page.

You **must** have a `<title>` tag in your HTML document for it to be considered
valid HTML. This `<title>` element must appear in the `<head>` section --
`<head>` is the only element that is considered a valid parent for `<title>`.
However, you should never have more than one `<title>` in your document.

 

Usage
-----

The following code snippet represents a valid use of `<title>`. Note its
location inside the `<head>` section and that exactly one `<title>` is present:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
<!DOCTYPE html>
<html>
    <head>
        <title>Baubles, Sundries, and Nonpareils</title>
    </head>

    <body>
    </body>
</html>
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The `<title>` tag does not support any element-specific attributes. It has only
global attributes, shared by all HTML elements (e.g. `class`, `id`, `lang`,
`style` ...) and event handler content attributes, which leverage JavaScript
triggered by specific events, and are also shared by nearly all HTML elements
(e.g. `onblur`, `onclick`, `onmouseover`).

 

### Browser Compatibility

The `<title>` tag works on all browsers and browser versions.

 

Special Notes
-------------

The `<title>` tag is considered a relatively important one for SEO purposes, and
as such, there is a wide variety of tips and hypotheses about how best to
strategically employ it to please the likes of Google and Bing.

Among the more common tips for writing a good `<title>` tag are:

-   Google will generally display the first 50-60 characters of a title, or as
    many as will fit into a 512-pixel display -- it is therefore recommended
    that you keep your `<title>` tag to under 55 characters (the number of
    characters recommended varies, but generally never exceeds 80).

-   Your title should be front-loaded with the most important keywords for your
    page. However, don’t spam your `<title>` tag with a long list of every
    conceivable keyword or repetitious keywords. E.g.: **Good**: `Skin Care
    Products`. **Bad**: `skin care products skin products creams ointments
    lotions liniments unguents salves oils emollients poultices moisturizers
    exfoliants cosmetics balms`

-   Don’t use punctuation in your title to separate keywords, though pipes (`|`)
    are considered acceptable, and hyphens or em dashes are seen as well

-   Don’t write your title as a whole sentence or a long phrase, as this is
    likely to dilute your keywords

-   If you use a brand name, offset it with some kind of punctuation. A lot of
    magazines and newspapers do this, e.g.: `Why The New York Times’ Clinton
    Error Is a Big Deal - The Atlantic`

-   Remember that what Google displays for the title of your page is
    **query-dependent**. Sometimes, it won’t display your title verbatim, but
    will modify it with some kind of algorithmic secret sauce to better match
    what a user specifically searched for.

-   The `<title>` element should not contain other elements inside it, not even
    inline ones.
