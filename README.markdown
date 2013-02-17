#diff_match_patch
a re-packaging of the javascript library by Neil Fraser for use in server side javascript

##Installation

`npm install diff_match_patch` or `component install marcelklehr/diff_match_patch`

##Usage
You'll be using instances of the diff_match_patch class:

```
dmpmod = require('diff_match_patch') 
var dmp = new dmpmod.diff_match_patch();
text1= "I'm some text";
text2= "I'm some other text";
puts(dmp.diff_main(text1, text2)); //print the difference of the texts
```

(for more detailed documentation, as well as a complete overview of the API, please refer to the original [project site](http://code.google.com/p/google-diff-match-patch/) ).

## Legal
Copyright 2006 Google Inc.

Licensed under the Apache License, Version 2.0
