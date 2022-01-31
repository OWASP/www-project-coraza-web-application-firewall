---

layout: col-sidebar
title: OWASP Coraza Web Application Firewall
tags: modsecurity coraza coraza-waf web-application-firewall waf coreruleset modsec
level: 2
type: code
pitch: OWASP Coraza is a golang enterprise-grade WAF framework compatible with Modsecurity and OWASP Core Ruleset.

---

![Logo](/assets/images/logo-coraza-mascot.png)

OWASP Coraza is a golang enterprise-grade Web Application Firewall framework that supports Modsecurity's seclang language and is 100% compatible with OWASP Core Ruleset.

Enrich your web application's security with powerful rules that comprehensively enforce good cybersecurity behavior. 

OWASP Coraza can be imported as a library or used with one of our connectors like [coraza-server](https://github.com/jptosso/coraza-server) (grpc and spoa), [coraza-caddy](https://github.com/jptosso/coraza-caddy) (web server, reverse proxy), [docker](#) (using connector).

## Try OWASP Coraza

Try OWASP Coraza using [OWASP Core Ruleset Sandbox](#) or the [Coraza Playground](#).

```sh
curl -H "x-format-output: txt-matched-rules" \
 -H "x-backend: coraza-caddy" \
"https://sandbox.coreruleset.org/?search=<script>alert('CRS+Sandbox+Release')</script>"
```