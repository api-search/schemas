---
description: UpdateVcnDetails schema from oracle-cloud-networking-openapi.yaml
layout: schema
name: UpdateVcnDetails
properties_list:
- description: ''
  name: displayName
  type: string
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-update-vcn-details-schema.json
slug: networking-update-vcn-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-update-vcn-details-schema.json\",\n  \"title\": \"UpdateVcnDetails\",\n  \"description\": \"UpdateVcnDetails schema from oracle-cloud-networking-openapi.yaml\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-update-vcn-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: UpdateVcnDetails
---
