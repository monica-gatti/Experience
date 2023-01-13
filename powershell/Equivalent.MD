
## To download a file from a Uri ( by instance a JSON file) you can use the WGET equivalent in PowerShell
```
PS >Invoke-WebRequest -Uri https://dst-de.s3.eu-west-3.amazonaws.com/mongo_fr/zips.json -UseBasicParsing -OutFile zips.json
```
## To unzip a tar file
```
tar -xzf filename.tgz
```
## which equivalent
The Linux 'which' command seems mutated by 'where' in PS. I tried with python, postgres but no way. 
Finally 'get-command' worked for python and returned the path
```
get-command -all python
```
