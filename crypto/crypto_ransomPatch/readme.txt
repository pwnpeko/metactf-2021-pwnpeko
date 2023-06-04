referenced from https://ctftime.org/writeup/31773
using https://github.com/kimci86/bkcrack
and https://github.com/kokke/tiny-AES-c 

../bkcrack -C ransomware-final.zip -c AES/unlicense.txt -P plain.zip -p unlicense.txt

found password 

../bkcrack -C ransomware-final.zip -c AES/unlicense.txt -P plaintext.zip -p unlicense.txt
    bkcrack 1.5.0 - 2022-07-08
    [15:43:46] Z reduction using 679 bytes of known plaintext
    100.0 % (679 / 679)
    [15:43:46] Attack on 10629 Z values at index 63
    Keys: a71f05f4 18438c7b 1cf62c29
    72.5 % (7707 / 10629)
    [15:43:51] Keys
    a71f05f4 18438c7b 1cf62c29

got flag

../bkcrack -C ransomware-final.zip -c key -d flacc.txt -k a71f05f4 18438c7b 1cf62c29
    bkcrack 1.5.0 - 2022-07-08
    [15:48:14] Writing deciphered data flacc.txt (maybe compressed)
    Wrote deciphered data.

MetaCTF{license_is_hard_to_spell}