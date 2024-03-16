# Bash

## If statements

```
if condition
then
    echo "condition true"
else
    echo "condition false"
fi
```

## Test if command available

### case work it

```
if command -v <cmd> &> /dev/null
then
    echo "command available"
    <cmd> ...
else
    echo "command not available"
fi
```

### trap if not available

```
if ! command -v <cmd> &> /dev/null
then
    echo "<cmd> not available"
    exit 1
fi
```

## Get status of last command

```
status=$?

# if pipeline:
status="${PIPESTATUS[0]}" # note "${pipestatus[0]}" in zsh!!
```

## Autokill long running command

`timeout` is a utility from `coreutils`

```
# kill after 10s if still running
timeout 10 command
```
