Define strings

```shell
DIR_PATH="/mnt/multires/OutputMultires/Session3_7FPS_50_15KM/"
i=1
```

Define numbers

```shell
((i=1))
```

Echo command output

```shell
echo "$(ls)"
```

Watch changes in file count

```shell
for i in {1..9999}; do ls -al "$DIR_PATH" |  wc -l; sleep 5; done
```

Loop over files

```shell

# echo before run to be sure
for f in "$BASE_DIR"/*; do echo rm -r "$f"; done
```
