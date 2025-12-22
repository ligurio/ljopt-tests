### Lua samples

```sh
$ find samples/ -name '*.lua' | while read s; do echo $s; cat $s | ./bin/ljopt - > /dev/null; done | tee log.txt
```

```sh
$ find lua/ -name '*.lua' -print0 | xargs --null -i luajit {}
```
