# Bash

## Kill Process
```bash
# get the id of process on port 3000
sudo lsof -t -i:3000
# kill process of id 1234
sudo kill -9 1234
```

### Solution N°2
```bash
ps -edf | grep ${id/port/...}
kill ${third column}
```

## change right on folder/file
```bash
# -R -> recursivity : all files and folders
sudo chown fvlb5625:fvlb5625 -R .m2
```

## Encode to base64

```bash
echo -n "" | base64
```
