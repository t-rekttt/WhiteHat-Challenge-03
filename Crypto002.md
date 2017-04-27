### Crypto002 ###

> We have components of an RSA cryptosystem. Decrypt the cipher to get the flag.

> RSA info: 

> - https://vi.wikipedia.org/wiki/RSA_(m%C3%A3_h%C3%B3a) Vietnamese
> - https://en.wikipedia.org/wiki/RSA_(cryptosystem) English"

> Download RSA-info file here:

> http://material.wargame.whitehat.vn/challenges/3/Crypto002_c576122a778397b48fa2d0368e2e02a14df1db41.zip

Submit WhiteHat{sha1(flag)}

1. Sau khi tải file info về, mở lên được một số giá trị: n, p, q, e, c. Đây là các giá trị tham gia vào quá trình mã hóa RSA.
![](http://i.imgur.com/xojdqTs.png)
2. Để giải mã được cần tìm private key (d). Mình dùng công cụ [rsatool](https://github.com/ius/rsatool) để xử lý
![](http://i.imgur.com/7Oz3L9s.png)
3. Sau khi có đủ giá trị, ta tiến hành giải mã. Input data như trong ảnh chính là giá trị e đã được chuyển thành dạng hex. Sau khi giải mã ta lại được một chuỗi hex khác
![](http://i.imgur.com/6AiyB5W.png)
4. Giải mã chuỗi hex, ta được flag
![](http://i.imgur.com/EP2ruxw.png)

Flag: **WhiteHat{sha1(simple_rsa_decryption)}**

