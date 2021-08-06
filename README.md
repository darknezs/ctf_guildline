# CTF_guildline
คู่มือในการแข่ง CTF(เบื้องต้น) เก็บไว้อ่านเอง
# find flag commands
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
 ```sh
$ grep -roa "flag{.*}" foldername หรือ -Ril แต่จะโชว์แค่ขื่อไฟล์เท่านั้น
 ```
# Linux Privilege Escalation
 ```sh
 $ sudo -l
 ```
  ```sh
 $ find / perm +6000 2>/dev/null | grep '\bin\'
 ```
 - when found interested binaries from previous command https://gtfobins.github.io/
# Web
- ctrl+u
- ctrl+shift+i
- cookie
- .js ไฟล์
- /robots.txt
- .htaccess
- .DS_Store
- /sitemap.xml
- /admin
- /.git/HEAD
- try `cat index.php`   // input validation
- Can enter site by some IP use 'X-Forwarded-For'
  ```sh 
  $ curl --header "X-Forwarded-For: 8.8.8.8" url 
  ```
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
- stegoveritas
```sh
$ pip3 install stegoveritas
$ stegoveritas secret.png
```

# Cryptography
- found big integer : https://scwf.dima.ninja/
- CyberChef : https://gchq.github.io/CyberChef/
- find p, q : http://factordb.com/
- WingDing ⬧︎●︎♋︎⧫︎ : https://lingojam.com/WingDing
- Book Cipher : https://www.dcode.fr/book-cipher
- Keyed Caesar cipher : https://www.boxentriq.com/code-breaking/keyed-caesar-cipher
# Forensics
- Wireshark
  - Voip
  - follow stream
  - extract object
# Mobile
- try to read code at MainActivity class
- apktool d <.apk>

