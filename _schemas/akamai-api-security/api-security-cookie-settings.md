---
description: Contains the cookie settings for a configuration.
layout: schema
name: cookie-settings
properties_list:
- description: Choose the type of domain. The default recommended type is `automatic`. Otherwise, choose `fqdn` to use the current Fully Qualified Domain name, `legacy` to use the original way in which the domain wa
  name: cookieDomain
  type: string
- description: If all of your traffic uses HTTPS, specify `true`. This option sets the Secure flag on all security product cookies, which are then only included with HTTPS traffic. It also adds `SameSite=None` to mo
  name: useAllSecureTraffic
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-cookie-settings-schema.json
slug: api-security-cookie-settings
source_filename: api-security-cookie-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-cookie-settings-schema.json\",\n  \"title\": \"cookie-settings\",\n  \"description\": \"Contains the cookie settings for a configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cookieDomain\": {\n      \"description\": \"Choose the type of domain. The default recommended type is `automatic`. Otherwise, choose `fqdn` to use the current Fully Qualified Domain name, `legacy` to use the original way in which the domain was selected, or `psl` to use the public suffix list to identify a private domain.\",\n      \"enum\": [\n        \"automatic\",\n        \"fqdn\",\n        \"legacy\",\n        \"psl\"\n      ],\n      \"type\": \"string\"\n    },\n    \"useAllSecureTraffic\": {\n      \"description\": \"If all of your traffic uses HTTPS, specify `true`. This option sets the\
  \ Secure flag on all security product cookies, which are then only included with HTTPS traffic. It also adds `SameSite=None` to most bot management cookies, ensuring that recent browser versions submit the cookies with protected requests. The `SameSite=None` cookie setting is necessary for site architectures that involve cross-domain form submission or inclusion of cross-domain iframes.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-cookie-settings-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: cookie-settings
---
