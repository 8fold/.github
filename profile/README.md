# 8fold Software

## CommonMark for PHP extensions

The following libraries and packages work with [CommonMark for PHP](https://commonmark.thephpleague.com).

[Fluent Markdown for CommonMark](https://github.com/8fold/commonmark-fluent-markdown) allows users to interact with CommonMark using a fluent API. It offers `FluentCommonMark`, which gives you access to the built in extensions and configuration settings of CommonMark. The `Markdown` class extends `FluentCommonMark` giving added access to the 8fold CommonMark extensions.

- Extensions can be added straight to ComminMark
	- [Abbreviations (for CommonMark)](https://github.com/8fold/commonmark-abbreviations) which is both a markdown syntax and CommonMark extension for generating `<abbr>` elements in HTML from markdown using a human-readable syntax (`[.Long Text to Abbreviate](LTA)` becomes `<abbr title="Long Text to Abbreviate">LTA</abbr>`).
	- [Partials (for CommonMark)](https://github.com/8fold/commonmark-partials) is both a syntax and CommonMark extension for creating more dynamic Markdown.
	- [Accessible Heading Permalinks for CommonMark](https://github.com/8fold/commonmark-accessible-heading-permalinks) for building accessible heading permalinks based on the work of [Amber Wilson](https://amberwilson.co.uk/blog/are-your-anchor-links-accessible/)

Note: If you find yourself using mutliple instances of CommonMark, Fluent Markdown for CommonMark offers a `Container` class for easy access.