# cloudflare-dig

This is just a utility to get the value of DNS records in Cloudflare whose type are `A`, `AAAA`, or `CNAME`. Why I wrote
this is because it is quite tedious to check the real value of proxied Cloudflare DNS records. With this, I don't need
to go into the console and doing those many clicks.

Obviously, this utility only works if you have the access to the Cloudflare account.

Prerequisites:
1.  Cloudflare API token stored in an environment variable `CLOUDFLARE_API_TOKEN`
2.  The token has permission to:
    - User Memberships: Read
    - Zone DNS: Read

How to run:
```
./cloudflare-dig <DOMAIN>
```
