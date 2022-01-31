---

layout: col-sidebar
title: OWASP Coraza Web Application Firewall
tags: modsecurity coraza coraza-waf web-application-firewall waf coreruleset modsec
level: 2
type: code
pitch: OWASP Coraza is a golang enterprise-grade WAF framework compatible with Modsecurity and OWASP Core Ruleset.

---

<p align="center">
    <img src="/assets/images/logo-coraza-mascot.png" alt="logo" height="100vh" width="auto">
</p>

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

## Take control of your applications

Control your requests and response before processing by your server or your customer's browser by submitting the content to our 4 "phase processors."

![Rule Phases](/assets/images/execution_flow.png)

Parse multiple content types, like XML, JSON, Multipart, and urlencoded, and don't miss anything. Coraza can transform all of this into easily manageable variables.

Extend OWASP Coraza to achieve anything; our plugin framework allows you to extend any capability, like operators, actions, directives, body processors, and audit engines.

Don't miss anything; log everything you need in order to achieve compliance and complete visibility of your applications.