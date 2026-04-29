---
description: AssociateCertificateRequest schema from Amazon MediaConvert API
layout: schema
name: AssociateCertificateRequest
properties_list:
- description: ''
  name: Arn
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-associate-certificate-request-schema.json
slug: mediaconvert-api-associate-certificate-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-associate-certificate-request-schema.json\",\n  \"title\": \"AssociateCertificateRequest\",\n  \"description\": \"AssociateCertificateRequest schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The ARN of the ACM certificate that you want to associate with your MediaConvert resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-associate-certificate-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AssociateCertificateRequest
---
