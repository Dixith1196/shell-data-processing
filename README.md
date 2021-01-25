# shell-data-processing

## Curl data:

- This is the curl command I used to get my data.
```Powershell 
curl "http://shakespeare.mit.edu/romeo_juliet/full.html" -O "data.txt"
```

## Bash Commands:

- Transform each space ' ' into a return character '\12'
```Powershell
tr ' ' '\12' < returnedfile
```
- Pipe the output to sort
```Powershell
tr ' ' '\12' < returnedfile | sort
```
- Pipe the sorted output to uniq -c to count
```Powershell
tr ' ' '\12' < returnedfile | sort | uniq -c
```
- Pipe the reduced output to sort with -nr flag
```Powershell
tr ' ' '\12' < returnedfile | sort | uniq -c | sort -nr
```
- Redirect the output to result.txt
```Powershell
tr ' ' '\12' < returnedfile | sort | uniq -c | sort -nr > result.txt
```


