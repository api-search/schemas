---
description: GetSiteAddressOutput schema from Amazon Outposts
layout: schema
name: GetSiteAddressOutput
properties_list:
- description: ''
  name: SiteId
  type: object
- description: ''
  name: AddressType
  type: object
- description: ''
  name: Address
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-get-site-address-output-schema.json
slug: openapi-get-site-address-output
source_filename: openapi-get-site-address-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-get-site-address-output-schema.json\",\n  \"title\": \"GetSiteAddressOutput\",\n  \"description\": \"GetSiteAddressOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SiteId\": {\n      \"$ref\": \"#/components/schemas/SiteId\"\n    },\n    \"AddressType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressType\"\n        },\n        {\n          \"description\": \"The type of the address you receive. \"\n        }\n      ]\n    },\n    \"Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Address\"\n        },\n        {\n          \"description\": \" Information about the address. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-get-site-address-output-schema.json
tags:
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: GetSiteAddressOutput
---
