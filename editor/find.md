---
title: Find and Replace
---

{% include back.html title="Editor" path="/editor" %}

The Drafts editor supports advanced find and replace of text in a draft.

To use find and replace:

- Tap the keyboard row options button, then select the magnifying glass icon – or tap ⌘-F on an external keyboard).
- Enter the text string you wish to find, and optionally replacement text.
- Tap "Find" to locate occurrences of that text in the current draft.

Any results will be display below, with a preview of the text surrounding the found text, and an indicator of the line number where that text occurs. Each of these results has two commands:

- _Select_: Close the find results and jump to that result in the editor with its text selected.
- _Replace_: Replace that occurrence of the text with the value in the "Replace" field. This will also update the results of the find.

The _Replace all_ button at the top will replace every occurrence in the results.

{% include doc-image.html src="/editor/find.png" %}

### Advanced Options

In addition to basic finds, the find and replace feature has a couple of additional option, which can be viewed by tapping the "Show options" button. Including toggling whether the search is case-sensitive, and more importantly, the ability to enable regular expressions.

If you have advanced search needs and are not familiar with regular expressions, there are [some](http://www.zytrax.com/tech/web/regex.htm) [great](https://regex101.com/) [resources](https://github.com/OpenRefine/OpenRefine/wiki/Understanding-Regular-Expressions) around the web.

For those familiar, know that Drafts implementation is based on [NSRegularExpression](https://www.raywenderlich.com/30288/nsregularexpression-tutorial-and-cheat-sheet) and any documentation on its syntax is applicable. With regular expressions enabled, the replace value supports capture group expressions in the format `$n` where `n` is the match index. This can be very useful for swapping values and similar operations.

### Regular Expression Example

As a simplified example, assume a draft with the following content:

```
Smith, Jim
Jones, Jane
```

Using a regular expression of `^([A-Za-z]*), ?([A-Za-z]*)` in the find, would find two results. This expressions, roughly explained, says find alpha-characters, then a comma and optional space, and then any remaining alpha-characters following.  The parentheses indicate capture groups that can be re-used in the replacement value, using `$n` where n is the order of the capture groups. Running replace all on this find, with `$2 $1` in the replace text, would result in the draft:

```
Jim Smith
Jane Jones
```

The capture group values for each find result were substituted for the placeholders in the replace text, and effectively swapped.

A full explanation of regular expression is beyond this help page, but please [ask in the community forums](https://forums.getdrafts.com) for assistance.
