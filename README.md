# Atom Snippets PHP Debug
Useful Atom Snippets for debugging with PHP

## How to install:

- Open the Command Palette: cmd-shift-P
- Write "Open Your Snippets" and then, enter
- Paste the code:

## How to use:

- Hit a prefix and press enter or tab.

### Prefixes

- Prefix <kbd>E</kbd> for debugging with ```echo```;
- Prefix <kbd>P</kbd> for debugging with ```print_r```;
- Prefix <kbd>V</kbd> for debugging with ```var_dump```;
- Prefix <kbd>D</kbd> for debugging with ```debug_print_backtrace```;

### Code

```coffee
echo '<pre>' . 'teste' . '<br>'; exit('Fim');
echo '<pre>'; print_r('teste'); echo '<br>'; exit('Fim');
echo '<pre>'; var_dump('teste'}); echo '<br>'; exit('Fim');
echo '<pre>'; debug_print_backtrace(); echo '<br>'; exit('Fim');
```

For more information about this look the [Atom Documentation](https://atom.io/docs/latest/using-atom-snippets)
