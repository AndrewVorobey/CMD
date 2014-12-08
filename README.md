CMD
===
1.find . -name ".java" | xargs grep -L -l "import ru.hh.deathstar" > almost_harmless.txt

2.ps -eo pid,cmd|egrep '^\s{1}[0-9]{5}\s+' |grep '127.0.0.1' |sort -r

3.find . -name ".log" | xargs grep -l -i "error" |tee -i newfile.txt | xargs wc -c
