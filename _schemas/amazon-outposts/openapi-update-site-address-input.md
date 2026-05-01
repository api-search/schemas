---
description: UpdateSiteAddressInput schema from Amazon Outposts
layout: schema
name: UpdateSiteAddressInput
properties_list:
- description: ''
  name: AddressType
  type: object
- description: ''
  name: Address
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-update-site-address-input-schema.json
slug: openapi-update-site-address-input
source_filename: openapi-update-site-address-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-update-site-address-input-schema.json\",\n  \"title\": \"UpdateSiteAddressInput\",\n  \"description\": \"UpdateSiteAddressInput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddressType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressType\"\n        },\n        {\n          \"description\": \" The type of the address. \"\n        }\n      ]\n    },\n    \"Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Address\"\n        },\n        {\n          \"description\": \" The address for the site. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AddressType\",\n    \"Address\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-update-site-address-input-schema.json
tags:
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: UpdateSiteAddressInput
---
