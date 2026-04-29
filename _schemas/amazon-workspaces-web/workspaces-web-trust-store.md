---
description: A trust store that can be associated with a web portal. A trust store contains certificate authority (CA) certificates. Once associated with a web portal, the browser in a streaming session will recognize certificates that have been issued using any of the CAs in the trust store. If your organization has internal websites that use certificates issued by private CAs, you should add the private CA certificate to the trust store.
layout: schema
name: TrustStore
properties_list:
- description: ''
  name: associatedPortalArns
  type: object
- description: ''
  name: trustStoreArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-trust-store-schema.json
slug: workspaces-web-trust-store
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"associatedPortalArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnList\"\n        },\n        {\n          \"description\": \"A list of web portal ARNs that this trust store is associated with.\"\n        }\n      ]\n    },\n    \"trustStoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the trust store.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A trust store that can be associated with a web portal. A trust store contains certificate authority (CA) certificates. Once associated with a web portal, the browser in a streaming session will recognize certificates that have been issued using any of the CAs in the trust store. If your organization has internal websites that use certificates issued by private CAs, you should add the private CA certificate to the trust store.\
  \ \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TrustStore\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-trust-store-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-trust-store-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: TrustStore
---
