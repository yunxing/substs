# substs
Replace a varaiable in a file to environment variable.

For example, if we have a file `META.in`:
```
version = "%{version}%"
...
```

`env version=0.0.6 substs META.in` will produce a file `META`:
```
version = "0.0.6"
...
```


