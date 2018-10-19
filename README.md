# Lab: Browsing the web with the terminal
Using the terminal to browse the web

## In this lab you will accomplish the following
 - Use the terminal to browse the web
 - Explore different status codes

## Use the application "curl"
 - Open the terminal
 - The usage of curl is: ```curl -v "[url]"```
 - If necessary install curl by following the instructions given when you try to launch the curl command
 - For example, entering ```curl -v "https://www.google.com"``` would have the subsequent result:

```
* Trying 172.217.5.68...
* TCP_NODELAY set
* Connected to www.google.com (172.217.5.68) port 443 (#0)
* TLS 1.2 connection using TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256
* Server certificate: www.google.com
* Server certificate: Google Internet Authority G2
* Server certificate: GeoTrust Global CA
> GET / HTTP/1.1
> Host: www.google.com
> User-Agent: curl/7.54.0
> Accept: */*
> 
< HTTP/1.1 200 OK
< Date: Fri, 22 Sep 2017 19:45:50 GMT
< Expires: -1
< Cache-Control: private, max-age=0
< Content-Type: text/html; charset=ISO-8859-1
< P3P: CP="This is not a P3P policy! See https://www.google.com/support/accounts/answer/151657?hl=en for more info."
< Server: gws
< X-XSS-Protection: 1; mode=block
< X-Frame-Options: SAMEORIGIN
< Set-Cookie: NID=112=NBVb7hjEG5Y2-jNvczgktDkk1SAKRnE6hLKA6c2pAWU7Y-iTHVGXOYWyjIDfaACqOP820vE9ysAkmOhtox2NxsjsVRhgXB2OAg3gE7awyR51OEv2n9E5G1u_hkMJQb3R; expires=Sat, 24-Mar-2018 19:45:50 GMT; path=/; domain=.google.com; HttpOnly
< Alt-Svc: quic=":443"; ma=2592000; v="39,38,37,35"
< Accept-Ranges: none
< Vary: Accept-Encoding
< Transfer-Encoding: chunked
< 
<!doctype html><html itemscope="" itemtype="http://schema.org/WebPage" lang="en">
...
```

## Answer the following questions in a text file called "answers.txt" at the root of this repository
  - For the domain www.google.com" using the scheme "http" 
    - What is the return code for the path "/" ?
    - What is the return code for the path /intl/en/policies/terms/?
  - For the domain "google.com" using the scheme "https"
    - What is the return code for the path "/"
        - If the path "/" for the domain "google.com" was entered into the browser what would happen? Write down the curl command that would simulate the HTTP request the browser would execute.
    - What is the return code for the path "/terms"
 - What is the return code for http://www.google.com/teapot?

