> openssl s_client -brief -connect baidu.com:443

> 查询网站证书过期时间
> echo | openssl s_client  -connect www.do-pp.icu:443 2> /dev/null | openssl x509 -noout -dates

> openssl x509 -text -noout -in selfsigned.crt # 查看证书信息

## Cryptographic Fundamentals

+ Symmetrical Encryption
  + DES(56 bit)
  + Triple DES(three times of DES)
  + AES(128 bit)
+ Asymmetrical Encryption
  + RSA(1024,2048, 4096)
  + ed25519

### Hashing Algorithms
  + MD5(128 bit)
  + SHA-1(160 bit)
  + SHA-2(256,384, 512 bit)
  + RIPEMD(128, 160,256, 320 bits)

### HMAC(Hashed Message Authentication Code)
### Digital Signatures

## CA 

> digicert
> let's encrypt

> crt.sh
> https://certificate.transparency.dev/
> https://www.ssllabs.com/

## TLS Handshake

> openssl ciphers -v

## SSL/TLS Vulnerabilities & Attacks

+ Downgrade Attack
+ Man in the Middle Attack
+ Poodle(Padding Oracle on Downgraded Legacy Encryption)
+ FREAK
+ SLOTH
+ Logjam
+ BEAST
+ Heartbleed








