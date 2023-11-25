# Markdown Test

README file to test every markdown parser/renderer/builder/etc out there.
Getting tired to look for this file everytime I need to test a program that
work with markdown.
Also included some extra test for common plugin.

Some idea come from [Markdown Cheatsheet · adam-p/markdown-here Wiki](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

Also see [CommonMark spec](https://spec.commonmark.org/). Read latest version, and section "Why is a spec needed?".

Anything after [Inline HTML](#inline-html) mostly not universal.
Syntax taken from:
- [Markdown it!](https://github.com/markdown-it)
- [kramdown](https://github.com/gettalong/kramdown)

## Header

# h1 `<some-code>`

## h2 *em*

### h3 **strong**

#### h4 ~~strike~~

##### h5 <u>HTML</u>

###### h6

alt h1
===

alt h2
---

## Emphasis

Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~

## List
```
This is inconsistent between any parser.
Sometime need 1 space for sub-list,
but sometime more. Investigate more.
in GFM (dot as space):
# this work
1. List item
...* Sub-list item
# this is not (when I create this doc)
1. List item
.* Sub-list item
```

1. First ordered list item
2. Another item
   * Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
   1. Ordered sub-list
4. And another item.

   You can have properly indented paragraphs within list items.
   Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

   To have a line break without a paragraph, you will need to use two trailing spaces.  
   Note that this line is separate, but within the same paragraph.  
   (This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

## Links

[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and
sometimes example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

## Images

Hover to see the title text):

```![alt](image src "title")```

Inline-style:
![GitHub logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png "GitHub logo")

```
![alt text][reference]

[reference]: image src "title"
```

Reference-style:
![GitHub logo][gh-logo]

[gh-logo]: https://github.githubassets.com/images/modules/logos_page/GitHub-Logo.png "GitHub logo"

Line break: \
![GitHub logo][gh-logo]

![Image only][gh-logo]

## Code and Syntax Highlighting

This is inline code: `Im inline code`

```css
html {
  color: #000;
  color: rgb(0,0,0);
}

custom-element {
  display: none;
}
```

## Table

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes `|` are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

## Blockquote

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 

## Horizontal Rule

Three or more...

---

Hyphens

***

Asterisks

___

Underscores

## Line Break

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

This line is also a separate paragraph, but  
This line is only separated by a single newline, so it's a separate line in the *same paragraph*.

This time we use \
GFM line break.

## Inline HTML

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

---

Most extended stuff below are not universal.


## Definition list

[Quick Reference | kramdown](https://kramdown.gettalong.org/quickref.html)

```md
term
: definition
: another definition

another term
and another term
: and a definition for the term
```

term
: definition
: another definition

another term
and another term
: and a definition for the term

## Block IAL

> A nice blockquote
{: #blockquote-id .blockquote-class title="Blockquote title"}

## Footnote

This is a text with a
footnote[^1].

[^1]: And here is the definition.

## `<sub>` and `<sup>`

[markdown-it/markdown-it-sub](https://github.com/markdown-it/markdown-it-sub) \
[markdown-it/markdown-it-sup](https://github.com/markdown-it/markdown-it-sup)

29^th^

H~2~O

29<sup>th</sup>

H<sub>2</sub>0

## Abbreviation

[markdown-it/markdown-it-abbr](https://github.com/markdown-it/markdown-it-abbr)

*[HTML]: Hyper Text Markup Language
*[W3C]:  World Wide Web Consortium

The HTML specification
is maintained by the W3C.

The <abbr title="Hyper Text Markup Language">HTML</abbr> specification
is maintained by the <abbr title="World Wide Web Consortium">W3C</abbr>.

## `<kbd>`

[jGleitz/markdown-it-kbd](https://github.com/jGleitz/markdown-it-kbd)

[[x]]

<kbd>x</kbd>

## `<ins>`

[markdown-it/markdown-it-ins](https://github.com/markdown-it/markdown-it-ins)

++inserted++

<ins>inserted</ins>

## `<mark>`

[markdown-it/markdown-it-mark](https://github.com/markdown-it/markdown-it-mark)
  
==marked==

<mark>marked</mark>
