# 8fold Software

## HTML Builder for PHP

[HTML Builder](https://github.com/8fold/php-html-builder) is a library designed to generate HTML strings, as opposed to ASTs or DOMs.

> I built and have used this library for years to eliminate DOM/AST memory overhead. Under PHP 8.5, its performance impact is practically invisible.
>
> ~ [Josh Bruce](https://github.com/joshbruce)

## XML Builder for PHP

[XML Builder](https://github.com/8fold/php-xml-builder) is a library designed to generate XML strings, as opposed to ASTs or DOMs.

It is the core library for:

- [Syndication](https://github.com/8fold/php-syndication) (specifically the Atom and RSS feeds) and
- [Sitemap](https://github.com/8fold/php-sitemap).

## CommonMark for PHP extensions

The following libraries and packages work with [CommonMark for PHP](https://commonmark.thephpleague.com).

[Fluent Markdown for CommonMark](https://github.com/8fold/commonmark-fluent-markdown) allows users to interact with CommonMark using a fluent API. It offers `FluentCommonMark`, which gives you access to the built in extensions and configuration settings of CommonMark. The `Markdown` class extends `FluentCommonMark` giving added access to the 8fold CommonMark extensions.

- Extensions can be added straight to CommonMark
	- [Abbreviations (for CommonMark)](https://github.com/8fold/commonmark-abbreviations) which is both a markdown syntax and CommonMark extension for generating `<abbr>` elements in HTML from markdown using a human-readable syntax (`[.Long Text to Abbreviate](LTA)` becomes `<abbr title="Long Text to Abbreviate">LTA</abbr>`).
	- [Partials (for CommonMark)](https://github.com/8fold/commonmark-partials) is both a syntax and CommonMark extension for creating more dynamic Markdown.
	- [Accessible Heading Permalinks for CommonMark](https://github.com/8fold/commonmark-accessible-heading-permalinks) for building accessible heading permalinks based on the work of [Amber Wilson](https://amberwilson.co.uk/blog/are-your-anchor-links-accessible/)

Note: If you find yourself using mutliple instances of CommonMark, Fluent Markdown for CommonMark offers a `Container` class for easy access.