# linuxcmd
These contain all the linux i migth need

# Curl commands 
```
curl -F "file=@file_name.txt" https://file.io`
```
> here the https://file.io can be any website where you want post the file to
---
```
echo "alias mdd ='cd ~/Desktop/mdd_dir'" >> ~/.bashrc
source ~/.bashrc
```
> Here instead `cd ~/Desktop/mdd_dir` could be any command you want execute so when you type mdd that command would executed here mdd can any name

```
ls -d .*/ 2>/dev/null
```

> To view all the hidden folders like .git/ directory which could found using this command and deleted if needed

```
xargs rm < a.txt
```

> To remove all the files in the file a.txt
> or 
```
xargs rm -rf < a.txt 
```
> for folders
---
```
xargs -a a.txt mv -t other
```

> here -a to specify the file and -t to specify target directory for the mv command


```
sort -u a.txt | xargs -I{} cp -r {} target_dir
```

> Here this will copy of the files and folders in a.txt to target_dir
