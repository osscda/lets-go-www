# Let's Go!

[![Azure Static Web Apps CI/CD](https://github.com/osscda/lets-go-www/workflows/Azure%20Static%20Web%20Apps%20CI/CD/badge.svg)](https://github.com/osscda/lets-go-www/actions?query=workflow%3A%22Azure+Static+Web+Apps+CI%2FCD%22)

The code for letsgocode.dev.

You'll need Hugo version 0.73.0 to run this site locally. To do it, run `hugo server`.

>This document is a work in progress.

(Powered by [Azure Static Web Apps](https://cda.ms/1s5))


# How to set up letsgocode.dev (without the www.)

https://docs.microsoft.com/en-us/azure/static-web-apps/custom-domain#configure-a-root-domain

- APEX domain
- Link to how to get APEX domains working: https://burkeholland.github.io/posts/static-app-root-domain/

# TODOs
- ✅ Go to cloudflare, set up the letsgocode.dev domain
- ✅ Set up DNS nameservers in porkbun:
    - `cory.ns.cloudflare.com`
    - `nicole.ns.cloudflare.com`
- ✅ Set up CNAME flattening
    - ✅ CNAME from `@` (root domain) to `www.letsgocode.dev` (make sure it's "proxied", not DNS only)
    - ✅ CNAME from `www` (subdomain) to the `black-field` Azure static web apps link
- LEFT OFF AT `page rules` header