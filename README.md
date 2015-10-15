# clitr

> Command Line Interface TRanslation.

Translate text in your terminal.

## Install

```
npm install -g clitr
```

## Usage

```
  Usage: clitr [options]

  Translate text in your terminal.

  Options:

    -h, --help         output usage information
    -V, --version      output the version number
    -l, --langs        list language code
    -f, --from <lang>  source language (default: auto)
    -t, --to <lang>    target language (default: en)
    -T, --text <text>  your text
    -s, --shell        run translation shell
```

## Examples

By default will translate from auto-detected language to English:
```
$ clitr -T 'Улыбаемся и машем! Мы мягкие и пушистые.'
Smile and wave! We are soft and fluffy.
```

What if you set the target language?:
```
$ clitr -t fr -T 'Show me the money!'
Montrez-moi l'argent!
```

The translation shell:
```
$ clitr -s
You are in translation shell.
To change translation direction input command "[<from>]:<to>" (e.g. ru:en).
> en:zh
Translation direction changed to en->zh.
> Hello world!
你好世界!
```

## License

MIT
