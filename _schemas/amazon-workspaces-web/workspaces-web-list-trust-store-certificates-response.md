---
description: ListTrustStoreCertificatesResponse schema from Amazon WorkSpaces Web API
layout: schema
name: ListTrustStoreCertificatesResponse
properties_list:
- description: ''
  name: certificateList
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: trustStoreArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-list-trust-store-certificates-response-schema.json
slug: workspaces-web-list-trust-store-certificates-response
source_filename: workspaces-web-list-trust-store-certificates-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateSummaryList\"\n        },\n        {\n          \"description\": \"The certificate list.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The pagination token used to retrieve the next page of results for this operation.&gt;\"\n        }\n      ]\n    },\n    \"trustStoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the trust store.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTrustStoreCertificatesResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-list-trust-store-certificates-response-schema.json\"\
  ,\n  \"description\": \"ListTrustStoreCertificatesResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-list-trust-store-certificates-response-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: ListTrustStoreCertificatesResponse
---
