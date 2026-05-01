---
description: Provides information about an entity that performed an action that produced a policy finding for a resource.
layout: schema
name: FindingActor
properties_list:
- description: ''
  name: domainDetails
  type: object
- description: ''
  name: ipAddressDetails
  type: object
- description: ''
  name: userIdentity
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-finding-actor-schema.json
slug: amazon-macie-finding-actor
source_filename: amazon-macie-finding-actor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-actor-schema.json\",\n  \"title\": \"FindingActor\",\n  \"description\": \"Provides information about an entity that performed an action that produced a policy finding for a resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainDetails\"\n        },\n        {\n          \"description\": \"The domain name of the device that the entity used to perform the action on the affected resource.\"\n        }\n      ]\n    },\n    \"ipAddressDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressDetails\"\n        },\n        {\n          \"description\": \"The IP address of the device that the entity used to perform the action on the affected\
  \ resource. This object also provides information such as the owner and geographic location for the IP address.\"\n        }\n      ]\n    },\n    \"userIdentity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdentity\"\n        },\n        {\n          \"description\": \"The type and other characteristics of the entity that performed the action on the affected resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-actor-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: FindingActor
---
