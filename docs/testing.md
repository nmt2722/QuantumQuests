# Testing all markdown extensions
## Abbreviations
Example usage 

The HTML specification is maintained by the W3C.
the sin, cos, tan and cot functions are worth learning.
so are cot and sec and cosec.
the abs value of ln or log of a function can be known by .....

## Admonitions
### Admonitions Basic
Admonitions, also known as call-outs, are an excellent choice for including side content without significantly interrupting the document flow. Material for MkDocs provides several different types of admonitions and allows for the inclusion and nesting of arbitrary content.

Example usage

!!! note

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
    This is a simple admonition !!! note.

!!! warning
    this is a warning admonition.
    Safety messages or hazard statements are known as admonitions
    usage is !!! warning and start typing the message on the next lines

!!! note "Phasellus posuere in sem ut cursus"

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa. Note with custom title
    The usage is !!! note "custom title"

!!! note ""
    This is an admonition without title and icon.
    !!! note "" is the usage

!!! example
    This is an example admonition which will be widely used.
    It will be further tested for latex katex embedding

!!! success
    This is a success admonition. !!! success is the usage
    Other admonitions are danger, bug, quote, question,failure, info,tips,abstract

### Collapsible Admonition

Using ??? instead of !!! will generate collapsible admonitons with toggle v.
Using ???+ will render exapnded admonition with toggle >

Example usage

??? tips
    This is a collapsible admonition not rendered.

???+ info
    This is an expanded admonition with an option to collapse.

### Inline Blocks

Example Usage 

!!! inline abstract "An abstract"
    Inline block admonition !!! inline classname "custom name" and text underneath.



!!! inline end danger "Red Danger box"
    This is inline end block !!! inline end classname "custom name" and text underneath.



??? inline quote "Quote"
    This is some quote.
    This inline and inline has bugs. 
    If i add anyblock it is inserted in between these blocks.
    I am figuring a way to resolve this problem.

!!! inline question "Question No 32"
    This is a question ?

!!! bug "Bug  with inline blocks"
    Random Texts to overcome the bugs.
    The Attribute Lists extension adds a syntax to define attributes on the various HTML elements in markdown’s output.
    This extension is included in the standard Markdown library.
    An example attribute list might look like this:
    {: #someid .someclass somekey='some value' }


## Definition Lists

Example usage 

`Definition`
: The definition is initiated by backticks `title of Definition` and in thie next line
a colon symbol is inserted : and the description of the definition is inserted.

## Buttons

Example usage
The following yntax is used to create buttons square brackets for texts followed by round brackets for the link and followed by flower brackets and .md-button .md-button--primary inserted inside

[Go to Home Page](./index.md){.md-button}

[Go to about page](./about.md){.md-button .md-button--primary}

[go to contact page :bus:](./contact.md){.md-button }

[Send :fontawesome-solid-paper-plane:](./index.md){ .md-button }

## Annotate

Annotations consist of two parts: a marker, which can be placed anywhere in a block marked with the annotate class, and content located in a list below the block containing the marker:

The marker is just a number in brackets and in the end inside the flower brackets dot anootate is typed. This is followed by a numbered list of values for the annotated numbers

This is how use anootations (1). There can be more than one annotation (2). Anootations are very useful (3).
{.annotate}

1. this is the first annotation.
2. :smile: this is the second one.
3. :rocket:This is the third annotation.

## Tabs

Example usage 

This is one of the most important md extensions for my projects.
The tabs are grouped under triple equal signs === "name" and content in the next line indented.

=== "Unordered list"

    * Sed sagittis eleifend rutrum
    * Donec vitae suscipit est
    * Nulla tempor lobortis orci

=== "Ordered list"

    1. Sed sagittis eleifend rutrum
    2. Donec vitae suscipit est
    3. Nulla tempor lobortis orci


## Grids

Example Usage
Grids come in two flavors: card grids, which wrap each element in a card that levitates on hover, and generic grids, which allow to arrange arbitrary block elements in a rectangular shape.

<div class="grid cards" markdown>

- :fontawesome-brands-html5: __HTML__ for content and structure
- :fontawesome-brands-js: __JavaScript__ for interactivity
- :fontawesome-brands-css3: __CSS__ for text running out of boxes
- :fontawesome-brands-internet-explorer: __Internet Explorer__ ... huh?

</div>


complex example

<div class="grid cards" markdown>

-   :material-clock-fast:{ .lg .middle } __Set up in 5 minutes__

    ---

    Install [`mkdocs-material`](#) with [`pip`](#) and get up
    and running in minutes

    [:octicons-arrow-right-24: Getting started](#)

-   :fontawesome-brands-markdown:{ .lg .middle } __It's just Markdown__

    ---

    Focus on your content and generate a responsive and searchable static site

    [:octicons-arrow-right-24: Reference](#)

-   :material-format-font:{ .lg .middle } __Made to measure__

    ---

    Change the colors, fonts, language, icons, logo and more with a few lines

    [:octicons-arrow-right-24: Customization](#)

-   :material-scale-balance:{ .lg .middle } __Open Source, MIT__

    ---

    Material for MkDocs is licensed under MIT and available on [GitHub]

    [:octicons-arrow-right-24: License](#)

</div>

