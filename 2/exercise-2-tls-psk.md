# Exercise 2: Securing a Channel with TLS and Pre-Shared Keys

You should now be able to retrieve keys from the KMS. In this step, the goal is to use the previously retrieved key `f7e0edef-8bf4-43b2-983b-1e9d22ca6f13` to establish a TLS 1.2 PSK (pre-shared key) connection.

A HTTPS server using TLS PSK is running at:

```text
tii-qkd-workshop.uaenorth.cloudapp.azure.com:4443
```

## Task

Write a TLS client, in a language of your choice, that can establish a TLS PSK connection with the server

Afterwards, over this channel, send an HTTP `GET` request to:

```text
/result
```

If everything works as expected, you should get an `HTTP/1.1 200 OK` response with `Content-Type: text/plain`. Write down the content of the HTTPS body

## Hints

1. More commonly, TLS is established with certificates. Find a library that allows using PSK instead of certificates
2. Use the actual 44-character Base64 string as the key, not the decoded byte string
