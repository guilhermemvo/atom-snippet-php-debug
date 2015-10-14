# Atom Snippets PHP Debug
Useful Atom Snippets for debugging with PHP

## How to install:

- Open the Command Palette: cmd-shift-P
- Write "Open Your Snippets" and then, enter
- Paste the code:

```coffee
'.source.php':

  'Debugging with echo':
    'prefix': 'e'
    'body':
      'echo \'<pre>\' . \'${1:teste}\' . \'<br>\'; exit(\'${2:Fim}\'); $3'

  'Debugging with print_r':
    'prefix': 'p'
    'body':
      'echo \'<pre>\'; print_r(${1:\'teste\'}); echo \'<br>$2\'; exit(\'${3:Fim}\'); $4'

  'Debugging with var_dump':
    'prefix': 'v'
    'body':
      'echo \'<pre>\'; var_dump(${1:\'teste\'}); echo \'<br>$2\'; exit(\'${3:Fim}\'); $4'

  'Debugging with debug_print_backtrace':
    'prefix': 'd'
    'body':
      'echo \'<pre>$1\'; debug_print_backtrace(); echo \'<br>\'; exit(\'${2:Fim}\'); $3'
```

## How to use:

- Hit a prefix and press enter or tab.

### Prefixes

#### Basic Invitation

- Prefix <kbd>E</kbd> for debugging with echo;
- Prefix <kbd>P</kbd> for debugging with print_r;
- Prefix <kbd>V</kbd> for debugging with var_dump;
- Prefix <kbd>D</kbd> for debugging with debug_print_backtrace;

### Code

```coffee
echo '<pre>' . 'teste' . '<br>'; exit('Fim');
echo '<pre>'; print_r('teste'); echo '<br>'; exit('Fim');
echo '<pre>'; var_dump('teste'}); echo '<br>'; exit('Fim');
echo '<pre>'; debug_print_backtrace(); echo '<br>'; exit('Fim');
```

For more information about this look the [Atom Documentation](https://atom.io/docs/latest/using-atom-snippets)
