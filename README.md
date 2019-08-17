# Xontrib Powerline 2
---

xontrib-powerline fork by [santagada/xontrib-powerline](https://github.com/santagada/xontrib-powerline).

<img src="https://github.com/6syun9/xontrib-powerline2/raw/master/img/example.png" alt="example" title="example">

# Install

```
pip install https://github.com/6syun9/xontrib-powerline2
```

And them load it on your ``.xonshrc``

```
xontrib load powerline
```


# Configuration

There are two variables that can be set, ``PL_PROMPT`` for the right prompt and ``PL_TOOLBAR`` for the bottom toolbar.
They contain a list of sections that can be used separated by ``>``. The value ``!`` means not to use that prompt.

Examples:

```
$PL_TOOLBAR = 'who>virtualenv>branch>cwd>full_proc'
$PL_TOOLBAR = '!'  # for no toolbar
xontrib load powerline
```

To see all available sections type ``pl_available_sections``, and to commit changes to your prompt execute ``pl_build_prompt``.

# Customize

- customize color: $PL_COLORS
- customize origin section: $PL_EXTRA_SEC

Examples:

```
$PL_COLORS = {"cwd": ("BLACK", "#a6e22e")}
$PL_EXTRA_SEC = {"user": lambda: [' {user} ', 'BLACK', '#fd971f']}
$PL_PROMPT='user>cwd>branch'
$PL_TOOLBAR='!'
$PL_RPROMPT='!'
xontrib load powerline
```

# Credits

This package was created by Leonardo Santagada with Cookiecutter_ 
and the `laerus/cookiecutter-xontrib`_ project template.

The font being used on the screenshot is the incredible `3270 font`_ with injected characters from `nerd fonts`_.

 - `nerd fonts`: https://github.com/ryanoasis/nerd-fonts
 - `3270 font`: https://github.com/rbanffy/3270font
 - `xontrib docs`: http://xon.sh/xontribs.html
 - `xontrib tutorial`: http://xon.sh/tutorial_xontrib.html
 - `Cookiecutter`: https://github.com/audreyr/cookiecutter
 - `laerus/cookiecutter-xontrib`: https://github.com/laerus/cookiecutter-xontrib