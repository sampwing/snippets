# Split a string using cut

Use cut to split strings into a list and retrieve a member

```
$ FOOBAR='foo bar'
$ FOO=`cut -f1 -d ' ' <<<$FOOBAR`
$ BAR=`cut -f2 -d ' ' <<<$FOOBAR`
$ echo $FOOBAR
foo bar
$ echo $FOO
foo
$ echo $BAR
bar
```
