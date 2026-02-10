

# 
A1 hashes to individual txt files into a custom directory called `hashes`
`haveibeenpwned-downloader.exe pwnedpasswords -s false`

### Download all NTLM hashes to a single txt file called `pwnedpasswords_ntlm.txt`
`haveibeenpwned-downloader.exe -n pwnedpasswords_ntlm`



## **Linux**


### Download all SHA1 hashes to a single txt file called `pwnedpasswords.txt` :
`haveibeenpwned-downloader pwnedpasswords`

### Download all SHA1 hashes to individual txt files into a custom directory called `hashes`:
`haveibeenpwned-downloader pwnedpasswords -s false`

### Download all NTLM hashes to a single txt file called `pwnedpasswords_ntlm.txt` : 
`haveibeenpwned-downloader -n pwnedpasswords_ntlm`



# Additional parameters

| Parameter   | Default value | Description |
|-------------|---------------|-------------|
| -s/--single | true | Determines whether to download hashes to a single file or as individual .txt files into another directory |
| -p/--parallelism | Same as `Environment.ProcessorCount` | Determines how many hashes to download at a time |
| -o/--overwrite | false | Determines if output files should be overwritten or not |
| -n | (none) | When set, the downloader fetches NTLM hashes instead of SHA1 |

# Additional usage examples
## Download all hashes to individual txt files into a custom directory called `hashes` using 64 threads to download the hashes
`haveibeenpwned-downloader.exe hashes -s false -p 64`
## Download all hashes to a single txt file called `pwnedpasswords.txt` using 64 threads, overwriting the file if it already exists
`haveibeenpwned-downloader.exe pwnedpasswords -o -p 64`
