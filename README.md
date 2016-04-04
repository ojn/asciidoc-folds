# asciidoc-folds package

This is a Asciidoc ported version of markdown-folder package.  

This package folds and unfolds asciidoc headings and fenced code blocks.

Note that the headings must use the equal signs. That is, underlined title formatting does not work.
There must also be some whitespace between the equal sign and the heading text. Examples that DO work:

`= My First Heading`

`== My Second Heading`

Commands:
  * 'asciidoc-folds:dwim-toggle': => Cycle headings if on a heading; toggle a fenced code block if on the first line; otherwise pass to the next key command
  * 'asciidoc-folds:toggle': => Fold/unfold heading at cursor
  * 'asciidoc-folds:unfoldall': => Unfold all headings
  * 'asciidoc-folds:cycle': => Cycle heading at cursor (Collapse all - show headings - show all)
  * 'asciidoc-folds:cycleall': => Cycle all h1 headings
  * 'asciidoc-folds:togglefenced': => Toggle folding of fenced code blocks
  * 'asciidoc-folds:toggleallfenced': => Toggle folding of all fenced code blocks
  * 'asciidoc-folds:unfoldall': => Unfold all headings
  * 'asciidoc-folds:foldall-h1': => Fold all h1 headings
  * 'asciidoc-folds:foldall-h2': => Fold all h2 headings
  * 'asciidoc-folds:foldall-h3': => Fold all h3 headings
  * 'asciidoc-folds:foldall-h4': => Fold all h4 headings
  * 'asciidoc-folds:foldall-h5': => Fold all h5 headings


Suggested bindings (not implemented, use in your personal settings if you like):

```
'atom-text-editor[data-grammar="source gfm"]:not([mini])':
  'tab':        'asciidoc-folds:dwim-toggle'
  'alt-c':      'asciidoc-folds:cycle'
  'ctrl-alt-c': 'asciidoc-folds:cycleall'
  'alt-x':      'asciidoc-folds:togglefenced'
  'ctrl-alt-x': 'asciidoc-folds:toggleallfenced'
  'alt-t':      'asciidoc-folds:toggle'
  'ctrl-alt-1': 'asciidoc-folds:foldall-h1'
  'ctrl-alt-2': 'asciidoc-folds:foldall-h2'
  'ctrl-alt-3': 'asciidoc-folds:foldall-h3'
  'ctrl-alt-4': 'asciidoc-folds:foldall-h4'
  'ctrl-alt-5': 'asciidoc-folds:foldall-h5'
```

Here is an example of an [mdpad](https://github.com/tshort/mdpad/tree/gh-pages)
markdown file with headings and many fenced code blocks. 

asciidoc-folds works the same but just with asciidoc syntax

![Folding in action](https://github.com/tshort/markdown-folder/raw/master/markdown-folder-mdpad.gif)
