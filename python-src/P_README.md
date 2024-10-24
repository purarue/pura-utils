Python functions that I like having installed globally so I can quickly import them from other scripts

`pura.notify`

```
>>>PMARK
perl -E 'print "`"x3, "python", "\n"'
python3 -c 'import pura.notify; help(pura.notify.notify)' | sed -e '1d' | chomp
perl -E 'print "`"x3', "\n\n"
```

`pura.jsonfast`: Speeds up JSON dump/load if [orjson](https://github.com/ijl/orjson) is installed. dumps also has a `minifed` flag which can compress JSON

```
>>>PMARK
perl -E 'print "`"x3, "python", "\n"'
python3 -c 'from pura.jsonfast import loads, dumps; help(loads); help(dumps)' | grep -v 'Help on function' | chomp
perl -E 'print "`"x3'
```

`pura.clipboard`: Python wrappers for `clipcopy` and `clippaste`:

```
>>>PMARK
perl -E 'print "`"x3, "python", "\n"'
python3 -c 'from pura.clipboard import clipcopy, clippaste; help(clipcopy); help(clippaste)' | grep -v 'Help on function' | chomp
perl -E 'print "`"x3'
```
