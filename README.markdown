# diff_match_patch

> A re-packaging of the [JavaScript library by Neil Fraser](https://code.google.com/p/google-diff-match-patch/).

The Diff Match and Patch libraries offer robust algorithms to perform the operations required for synchronizing plain text.

This library implements [Myer's diff algorithm](http://neil.fraser.name/software/diff_match_patch/myers.pdf) which is generally considered to be the best general-purpose diff. A layer of [pre-diff speedups and post-diff cleanups](http://neil.fraser.name/writing/diff/) surround the diff algorithm, improving both performance and output quality.

This library also implements a [Bitap matching algorithm](http://neil.fraser.name/software/diff_match_patch/bitap.ps) at the heart of a [flexible matching and patching strategy](http://neil.fraser.name/writing/patch/).

* [Diff](http://neil.fraser.name/software/diff_match_patch/svn/trunk/demos/demo_diff.html). Compare two blocks of plain text and efficiently return a list of differences.
* [Match](http://neil.fraser.name/software/diff_match_patch/svn/trunk/demos/demo_match.html). Given a search string, find its best fuzzy match in a block of plain text. Weighted for both accuracy and location.
* [Patch](http://neil.fraser.name/software/diff_match_patch/svn/trunk/demos/demo_patch.html). Apply a list of patches onto plain text. Use best-effort to apply patch even when the underlying text doesn't match.

## Installation

```
$ npm install diff_match_patch
... or
$ component install marcelklehr/diff_match_patch
... or
```

## Usage

You'll be using instances of the diff_match_patch class:

```javascript
var dmpmod = require('diff_match_patch');
var dmp = new dmpmod.diff_match_patch();

var text1 = "I'm some text";
var text2 = "I'm some other text";

console.log(dmp.diff_main(text1, text2)); // print the difference of the texts
```

For more detailed documentation, as well as a complete overview of the API, please refer to the original [project site](http://code.google.com/p/google-diff-match-patch/)).

## License

Copyright 2006 Google Inc. Licensed under the Apache License, Version 2.0.
