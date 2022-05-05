
How I Was Able To Takeover Any Virustotal Account
Hi Everyone,

I’m back with one of my recent findings. Well, As you guys already know that Google is a huge MNC and it’s security is tough as Hell. So, technically it’s hard to find something like a ‘security flaw’.

Honestly, it was my dream to get my name on the ‘Google Hall Of Fame’. I saw some leets are already there and they have their names published in news. So, I started with a subdomain enumeration using sublist3r. I got many subdomains, also searched about Google Subdomains online.

You may be aware about a subdomain name Virustotal.com.

As, I was going through the major subdomains and thought to pay virustotal.com a visit. I quickly opened virustotal.com and went through all the features and noted em one by one. I was in search of some low hanging fruits, but got nothing out of it. I was little disappointed by that so I took a break. When I resumed precisely after few hours, to my surprise I forgot my account password… -/

I visited the ‘forgot password’ page and keyed in my details and recived an e-mail. I copied that ‘password reset’ link and opned in new tab and intercepted that request.

Everything went as usual with nothing worth special attention, but then I noticed something in the request . I captured this request and sent it to the repeater.
I visited the ‘forgot password’ page again, but this time I entered my second account details. I received the ‘password reset’ link.
Then, I did the same as i did with my first account,

I replaced my second account username with my first account username.

![Alt text](https://raw.githubusercontent.com/ali-kaptanoglu/bug-bounty/main/Account-takeover/virustotal.png "virustotal")



And, I forwarded the request.
Then I chose a new password and entered it twice as required. After that I tried to login to my first account nothumanninja.

But it said ‘wrong password’

Oops! 😎

Then I tried the new password…
BOOOOM!!!

Successfully Logged In…
