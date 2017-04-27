### Crypto001 ###

I happen to get this text, but it seems to be encrypted. Decrypt it and find the hidden flag.
> HJXAJY GPHTPR HPL P CPBDG APGTCTV SCP CPXRXIXADE DWL LTGWIGTKD TWI CPBDG RXAQJETG SCP STWHXAQPIHT TWI TAJG UD TWI HGDGTEBT. GPHTPR STHJ TWI HBTAQDGE SCP HEXWHSGPW UD TWI SDXGTE DI TIPTGR HXW CLD TBTGEJH APRXIXADE SCP NGPIXAXB GTLDE. VPAU HX TWI GPTN IPWI GPHPTR HPL CGDQ. CPBDG GDGTEBT HJXAJY GPHTPR HX STSGPVTG HP TCD UD TWI IHDB AJUGTLDE SCP AJUHHTRRJH HGTSPTA CX TWI NGDIHXW UD TWI SAGDL. HXW TUXA SCP HXW ICTADXK WIPTS TKPW CTTQ NATSXL STIPGQTATR CX TGJIPGTIXA SCP BAXU.

Submit WhiteHat{sha1(flag)}

1. Nghi ngờ đoạn văn bản được mã hóa bằng Caesar/Subtitution, nên mình tiến hành phân tích bằng phần mềm CrypTool. Mở CrypTool, paste đoạn văn bản ban đầu, chọn Analysis -> Symmetric Encryption (basic) -> Ciphertext-Only -> Caesar. Phần mềm trả về kết quả tốt nhất (phần khoanh đỏ)
![](http://i.imgur.com/kfTuQSC.png)
2. Sau khi kiểm tra vài từ thì mình nhận ra rằng đoạn văn bản đã được đảo lại hết các từ và các tiếng trong câu. Viết 1 đoạn JS để đảo lại câu.
![](http://i.imgur.com/gcLu0MQ.png)
3. Tìm thấy gợi ý flag:
> FLAG IS THE YEAR THAT CAESAR WAS BORN
4. Google theo gợi ý là ra flag ngay :3

Flag: **WhiteHat(sha1(100))**