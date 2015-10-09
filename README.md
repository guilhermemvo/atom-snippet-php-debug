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
      'echo \'<pre>\' . \'$1\' . \'<br>\'; exit(\'${2:Fim}\'); $3'

  'Debugging with print_r':
    'prefix': 'p'
    'body':
      'echo \'<pre>\'; print_r(${1:\'teste\'}); echo \'<br>$2\'; exit(\'${3:Fim}\'); $4'

  'Debugging with var_dump':
    'prefix': 'v'
    'body':
      'echo \'<pre>\'; var_dump(${1:\'teste\'}); echo \'<br>$2\'; exit(\'${3:Fim}\'); $4'
```

For more information about this look the [Atom Documentation](https://atom.io/docs/latest/using-atom-snippets)
