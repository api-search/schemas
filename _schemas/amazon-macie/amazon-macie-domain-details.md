---
description: Provides information about the domain name of the device that an entity used to perform an action on an affected resource.
layout: schema
name: DomainDetails
properties_list:
- description: ''
  name: domainName
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-domain-details-schema.json
slug: amazon-macie-domain-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-domain-details-schema.json\",\n  \"title\": \"DomainDetails\",\n  \"description\": \"Provides information about the domain name of the device that an entity used to perform an action on an affected resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-domain-details-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: DomainDetails
---
