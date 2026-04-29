---
description: A cookie persistence profile that maintains session persistence by inserting or reading HTTP cookies.
layout: schema
name: CookiePersistenceProfile
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
- description: Whether to always send the cookie.
  name: alwaysSend
  type: string
- description: Cookie encryption method.
  name: cookieEncryption
  type: string
- description: Name of the persistence cookie.
  name: cookieName
  type: string
- description: Parent profile.
  name: defaultsFrom
  type: string
- description: ''
  name: description
  type: string
- description: Cookie expiration time.
  name: expiration
  type: string
- description: Length of the cookie hash.
  name: hashLength
  type: integer
- description: Offset for the cookie hash.
  name: hashOffset
  type: integer
- description: Whether the cookie has the HttpOnly flag.
  name: httponly
  type: string
- description: Whether to match persistence across pools.
  name: matchAcrossPools
  type: string
- description: Whether to match persistence across virtual servers.
  name: matchAcrossServices
  type: string
- description: Whether to match persistence across all virtuals.
  name: matchAcrossVirtuals
  type: string
- description: Cookie persistence method.
  name: method
  type: string
- description: Whether to mirror persistence records.
  name: mirror
  type: string
- description: Whether to override connection limits for persisted sessions.
  name: overrideConnectionLimit
  type: string
- description: Whether the cookie has the Secure flag.
  name: secure
  type: string
- description: Persistence timeout in seconds.
  name: timeout
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-cookie-persistence-profile-schema.json
slug: bigip-icontrol-rest-cookie-persistence-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CookiePersistenceProfile\",\n  \"type\": \"object\",\n  \"description\": \"A cookie persistence profile that maintains session persistence by inserting or reading HTTP cookies.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"fullPath\": {\n      \"type\": \"string\"\n    },\n    \"generation\": {\n      \"type\": \"integer\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\"\n    },\n    \"alwaysSend\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to always send the cookie.\"\n    },\n    \"cookieEncryption\": {\n      \"type\": \"string\",\n      \"description\": \"Cookie encryption method.\"\n    },\n    \"cookieName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the persistence cookie.\"\n    },\n    \"defaultsFrom\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Parent profile.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"expiration\": {\n      \"type\": \"string\",\n      \"description\": \"Cookie expiration time.\"\n    },\n    \"hashLength\": {\n      \"type\": \"integer\",\n      \"description\": \"Length of the cookie hash.\"\n    },\n    \"hashOffset\": {\n      \"type\": \"integer\",\n      \"description\": \"Offset for the cookie hash.\"\n    },\n    \"httponly\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the cookie has the HttpOnly flag.\"\n    },\n    \"matchAcrossPools\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to match persistence across pools.\"\n    },\n    \"matchAcrossServices\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to match persistence across virtual servers.\"\n    },\n    \"matchAcrossVirtuals\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to match persistence across all virtuals.\"\
  \n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"Cookie persistence method.\"\n    },\n    \"mirror\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to mirror persistence records.\"\n    },\n    \"overrideConnectionLimit\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to override connection limits for persisted sessions.\"\n    },\n    \"secure\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the cookie has the Secure flag.\"\n    },\n    \"timeout\": {\n      \"type\": \"string\",\n      \"description\": \"Persistence timeout in seconds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-cookie-persistence-profile-schema.json
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
title: CookiePersistenceProfile
---
