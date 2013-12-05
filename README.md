olga
====

*coming soon...*

A new approach to UI testing, because the usual approaches suck.

```coffee

div = document.querySelector '#div'

# olga: `div` should not be undefined

div.removeClass 'hide'

# olga: `div` should be visible

div.style.top = '100px'

# olga: `div.offsetTop` should be equal to `100px`
```

then on the command line,

```bash
olga script.coffee
```

which runs through the script, injecting olga calls based on parsed comments, and testing everything as it runs. this avoids annoying timing issues that plague current-generation ui testing frameworks.
