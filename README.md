# CTF_guildline
คู่มือในการแข่ง CTF(เบื้องต้น) เก็บไว้อ่านเอง
# find flag commarnds
```sh
$ strings <file> | grep "flag"
```
 ```sh 
 $ cat * | grep "flag" 
 ```
 ```sh 
 $ strings * | grep "flag" 
 ```
 ```sh
$ strings <file> | less
```
 ```sh
$ printf '%s' "$(<flag.txt)"
```

# Web
- ctrl+u
- ctrl+shift+i
- cookie
- .js ไฟล์
- /robots.txt
- /sitemap.xml
- /admin
# Steganography
- exiftool
```sh
$ exiftool <img file>
```
- binwalk
```sh
$ binwalk -e <img file>
```
- steghide
```sh
$ steghide extract -sf img
```


# Cryptography
- found big integer : https://scwf.dima.ninja/
- CyberChef : https://gchq.github.io/CyberChef/
# Forensics

