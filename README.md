# [interactive shell for blockdiag](http://interactive.blockdiag.com/)

- Works like [blockdiag](http://blockdiag.com/) web editor
- Simple WSGI Apps (using Flask)
- Hosted on Google Appengine

- Limitations:
    - All diagram sources are saved as URL parameter, not any databases
    - Could not render large diagram (it raises URL length overflow)

Author: @tk0miya <i.tkomiya at gmail.com>

## How to run locally (for debugging)

```
$ git clone https://github.com/blockdiag/blockdiag_interactive_shell
$ cd blockdiag_interactive_shell
$ python bootstrap.py
$ bin/buildout
$ bin/dev_appserver app
```

And then, access http://localhost:8080/
