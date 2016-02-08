HTML tags are made up of characters that sit inside angled brackets. An HTML tags consists of an opening tag, the corresponding closing tag, and the text in between They give the information they surround special meaning. Opening tags can carry attributes, which tell us more about the content of that element. Attributes require a name and a value.

## `<html>`

Defines the document's root element. Each HTML document contains only one root element. All other elements must go inside the root element, except for [`<!DOCTYPE>`](#doctype).

* _parents_: none, it's the top
* _content_: _only_ [`<head>`](#head) and [`<body>`](#body)
* _display_: `block`, maybe? I mean, I can see it... RESEARCH!


## `<head>`

Defines the document's head element. The browser does not display this element, which only carries metadata like the title and description. Browsers can use metadata to enhance the user's experience, and we'll discuss it later on.

* _parents_: ['<HTML>'](#HTML) element, as its first child
* _content_: one or more elements of metadata content where exactly one is a <title> element
* _category_: none

* _attributes_:

`profile` -- The URIs of one or more metadata profiles, separated by white space


## `<body>`

Defines the document's body element. There is only one body element inside an HTML document and it always comes after the head element. Everything the user will see goes in the body element.

* _parents_: must be the second element of an ['<html>'](#html) element
* _content_: [Flow Contant][1]
* _category_: sectioning root

* _attributes_:

`background` -- URI of a image to use as a background
`top-margin` -- The margin of the top of the body
`right-margin` -- The margin of the right of the body
`bottom-margin` -- The margin of the bottom of the body
`left-margin` -- The margin of the left of the body
`text` -- Foreground color of text


## `<title>`

Defines the document's title element. The title element is the only mandatory HTML element, and it goes inside the head element since the title is part of the metadata shown in various places (such as the browser tab or as part of a search engine result).


* _parents_: A ['<head>'](#head) element that contains no other <title> element.
* _content_: Text that is not inter-element whitespace
* _category_: metadata content


## `<!DOCTYPE html>`

The doctype is a formal declaration, placed at the very start of an HTML document, that the document is a standard HTML document.

* _category_: none


## `<!- -  and  - ->`

Comments are notes you put in your HTML document for your own needs.

* _category_: none


## `<a>`

This tag is used to create a link to external resources such as a different webpage, an email, an image, a different section of the current document, and so on.

* _parents_: Any element that accepts phrasing content, or any element that accepts [Flow Contant][1]
* _content_: transparent, containing either [Flow Contant][1] or phrasing content
* _display_: `inline`
* _category_: any [Flow Contant][1], palpable content, phrasing content, interactive content

* _attributes_:

`href` -- single required attribute for anchors defining a hypertext source link
`rel` -- this attribute specifies the relationship of the target object to the link object.
`type` -- Indicates the numbering type
`target` -- specifies where to display the linked resource


## `<article>`

Represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable

* _parents_: Any element that accepts [Flow Contant][1]
* _content_: any [Flow Contant][1]
* _category_: [Flow Contant][1], sectioning content, palpable content.


## `<div>`

HTML Document Division Element is the generic container for flow content, which does not inherently represent anything. It can be used to group elements for styling purposes or because they share attribute values. It should be used only when no other semantic element is appropriate.

* _parents_: anything that accepts [Flow Content][1], which is apparently a lot of things.
* _content_: any [Flow Contant][1], palpable content (WTF?)
* _display_: `block`


## `<footer>`

Represents a footer for its nearest sectioning content or sectioning root element. A footer typically contains information about the author of the section, copyright data or links to related documents.

* _parents_: Any element that accepts [Flow Contant][1]
* _content_: [Flow Contant][1] but with no ['<footer>'](#footer) or ['<header>'](#header) descendants
* _category_:[Flow Contant][1], palpable content


## `<header>`

Represents a group of introductory or navigational aids. It may contain some heading elements but also other elements like a logo, wrapped section's header, a search form, and so on. <h1>, <h2>, <h3>, <h4>, <h5>, <h6> These tags define headings, ranging from h1 for the most general heading to h6 for the most 		specific.

* _parents_: Any element that accepts [Flow Contant][1]
* _content_: [Flow Contant][1] but with no ['<footer>'](#footer) or ['<header>'](#header) descendants
* _display_: `block`
* _category_: [Flow Contant][1], palpable content

## `<nav>`

Represents a section of a page that links to other pages or to parts within the page: a section with navigation links.

* _parents_: Any element that accepts [Flow Contant][1]
* _content_: [Flow Contant][1]
* _category_: [Flow Contant][1], sectioning content, palpable content


## `<ol>`

Represents an ordered list of items.

* _parents_: Any element that accepts [Flow Contant][1]
* _content_: Zero or more ['<li>'](#li) elements
* _display_: `block`
* _category_: [Flow Contant][1], and if the ['<ol>'](#ol) element's children include at least one

* _attributes_:

`start` --  specifies the start value for numbering the individual list items.
`type` -- Indicates the numbering type


## `<p>`

This is the paragraph tag, used to create paragraphs, which are usually separated by line breaks.

* _parents_: any element that excepts [Flow Contant][1]
* _content_: Phrasing content
* _display_: `block`
* _category_: [Flow Contant][1], palpable content


## `<strong>`

Gives text strong importance, and is typically displayed in bold.

* _parents_: Any element that accepts phrasing content, or any element that accepts [Flow Contant][1]
* _content_: phrasing content
* _display_: `inline`
* _category_: [Flow Contant][1], phrasing content


## `<span>`

A generic inline container for phrasing content that can be used to group elements for styling purposes, or because they share attribute values, such as lang. It should be used only when no other semantic element is appropriate. <span> is very much like a <div> element, but <div> is a block-level element whereas a <span> is an inline element.

* _parents_: Any element that accepts phrasing content, or any element that accepts [Flow Contant][1]
* _content_: Phrasing content
* _category_:[Flow Contant][1], phrasing content


## `<ul>`

Represents an unordered list of items, namely a collection of items that do not have a numerical ordering, and their order in the list is meaningless.

* _parents_: Any element that accepts [Flow Contant][1]
* _content_: zero or more ['<li>'](#li) elements, eventually mixed with ['<ol>'](#ol) and ['<ul>'](#ul) elements.
* _display_: `block`
* _category_: [Flow Contant][1]

* _attributes_:

`type` -- Used to set the bullet style for the list.

###### Footnotes

[1](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Flow_content)
