---
description: An HTTP profile that defines how the BIG-IP processes HTTP traffic for a virtual server.
layout: schema
name: HttpProfile
properties_list:
- description: ''
  name: kind
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: fullPath
  type: string
- description: ''
  name: generation
  type: integer
- description: ''
  name: selfLink
  type: string
- description: Whether to accept X-Forwarded-For headers from clients.
  name: acceptXff
  type: string
- description: ''
  name: appService
  type: string
- description: Realm for HTTP Basic authentication challenges.
  name: basicAuthRealm
  type: string
- description: Parent profile from which this profile inherits settings.
  name: defaultsFrom
  type: string
- description: ''
  name: description
  type: string
- description: List of cookie names to encrypt.
  name: encryptCookies
  type: array
- description: ''
  name: enforcement
  type: object
- description: Fallback host for HTTP redirects.
  name: fallbackHost
  type: string
- description: HTTP status codes that trigger fallback redirection.
  name: fallbackStatusCodes
  type: array
- description: Regular expression for headers to remove from responses.
  name: headerErase
  type: string
- description: Header to insert into requests.
  name: headerInsert
  type: string
- description: Whether to insert an X-Forwarded-For header.
  name: insertXforwardedFor
  type: string
- description: Whether to rewrite HTTP connections for OneConnect.
  name: oneconnectTransformations
  type: string
- description: Redirect rewrite mode.
  name: redirectRewrite
  type: string
- description: How to handle chunked requests.
  name: requestChunking
  type: string
- description: How to handle chunked responses.
  name: responseChunking
  type: string
- description: Server agent string to include in responses.
  name: serverAgentName
  type: string
- description: Hostname to use in Via headers.
  name: viaHostName
  type: string
- description: Via header handling for requests.
  name: viaRequest
  type: string
- description: Via header handling for responses.
  name: viaResponse
  type: string
- description: Alternative header names for X-Forwarded-For.
  name: xffAlternativeNames
  type: array
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-http-profile-schema.json
slug: bigip-icontrol-rest-http-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HttpProfile\",\n  \"type\": \"object\",\n  \"description\": \"An HTTP profile that defines how the BIG-IP processes HTTP traffic for a virtual server.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"fullPath\": {\n      \"type\": \"string\"\n    },\n    \"generation\": {\n      \"type\": \"integer\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\"\n    },\n    \"acceptXff\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to accept X-Forwarded-For headers from clients.\"\n    },\n    \"appService\": {\n      \"type\": \"string\"\n    },\n    \"basicAuthRealm\": {\n      \"type\": \"string\",\n      \"description\": \"Realm for HTTP Basic authentication challenges.\"\n    },\n    \"defaultsFrom\": {\n      \"type\": \"string\",\n      \"description\": \"Parent profile from which this\
  \ profile inherits settings.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"encryptCookies\": {\n      \"type\": \"array\",\n      \"description\": \"List of cookie names to encrypt.\"\n    },\n    \"enforcement\": {\n      \"type\": \"object\"\n    },\n    \"fallbackHost\": {\n      \"type\": \"string\",\n      \"description\": \"Fallback host for HTTP redirects.\"\n    },\n    \"fallbackStatusCodes\": {\n      \"type\": \"array\",\n      \"description\": \"HTTP status codes that trigger fallback redirection.\"\n    },\n    \"headerErase\": {\n      \"type\": \"string\",\n      \"description\": \"Regular expression for headers to remove from responses.\"\n    },\n    \"headerInsert\": {\n      \"type\": \"string\",\n      \"description\": \"Header to insert into requests.\"\n    },\n    \"insertXforwardedFor\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to insert an X-Forwarded-For header.\"\n    },\n    \"oneconnectTransformations\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Whether to rewrite HTTP connections for OneConnect.\"\n    },\n    \"redirectRewrite\": {\n      \"type\": \"string\",\n      \"description\": \"Redirect rewrite mode.\"\n    },\n    \"requestChunking\": {\n      \"type\": \"string\",\n      \"description\": \"How to handle chunked requests.\"\n    },\n    \"responseChunking\": {\n      \"type\": \"string\",\n      \"description\": \"How to handle chunked responses.\"\n    },\n    \"serverAgentName\": {\n      \"type\": \"string\",\n      \"description\": \"Server agent string to include in responses.\"\n    },\n    \"viaHostName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname to use in Via headers.\"\n    },\n    \"viaRequest\": {\n      \"type\": \"string\",\n      \"description\": \"Via header handling for requests.\"\n    },\n    \"viaResponse\": {\n      \"type\": \"string\",\n      \"description\": \"Via header handling for responses.\"\n    },\n    \"\
  xffAlternativeNames\": {\n      \"type\": \"array\",\n      \"description\": \"Alternative header names for X-Forwarded-For.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-http-profile-schema.json
tags:
- API Gateway
- Application Delivery
- Automation
- Edge Computing
- Kubernetes
- Load Balancing
- Multi-Cloud
- NGINX
- Security
- WAF
title: HttpProfile
---
