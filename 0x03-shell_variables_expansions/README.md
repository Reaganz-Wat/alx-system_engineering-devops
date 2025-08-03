## Script Commands Documentation

### 0-alias
Creates an alias `ls` that deletes all files in the current directory:
```bash
alias ls='rm *'
```

### 1-hello_you
Prints a greeting with the current username:
```bash
echo "hello $(whoami)"
```

### 2-path
Adds `/action` to the `PATH` environment variable:
```bash
export PATH="$PATH:/action"
```

### 3-paths
Counts the number of directories in the `PATH` variable:
```bash
echo "$PATH" | tr ':' '\n' | wc -l
```

### 4-global_variables
Prints all global environment variables:
```bash
printenv
```

### 5-local_variables
Prints all shell variables, including local ones:
```bash
set
```

### 6-create_local_variable
Creates a local variable `BEST` with value `School`:
```bash
BEST='School'
```

### 7-create_global_variable
Creates a global variable `BEST` with value `School`:
```bash
BEST='School'
```

### 8-true_knowledge
Adds 128 to the value of `TRUEKNOWLEDGE` and prints the result:
```bash
echo $((TRUEKNOWLEDGE + 128))
```

### 9-divide_and_rule
Divides the value of `POWER` by `DIVIDE` and prints the result:
```bash
echo $(( $POWER / $DIVIDE ))
```

### 10-love_exponent_breath
Raises `BREATH` to the power of `LOVE` and prints the result:
```bash
echo $(($BREATH**$LOVE))
```

### 11-binary_to_decimal
Converts the value of `BINARY` from binary to decimal and prints the result:
```bash
echo $((2#$BINARY))
```

### 12-combinations
Prints all two-letter combinations from `a` to `z`, except `oo`:
```bash
for i in {a..z}
do
  for j in {a..z}
  do
    [ $i$j = oo ] && continue
    echo $i$j
  done
done
```

### 13-print_float
Prints the value of `NUM` as a float with two decimal places:
```bash
printf "%.2f\n" "$NUM"
```
