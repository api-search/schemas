---
description: Placeholder documentation for PurchaseOfferingResponse
layout: schema
name: PurchaseOfferingResponse
properties_list:
- description: ''
  name: Reservation
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-purchase-offering-response-schema.json
slug: medialive-api-purchase-offering-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-purchase-offering-response-schema.json\",\n  \"title\": \"PurchaseOfferingResponse\",\n  \"description\": \"Placeholder documentation for PurchaseOfferingResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Reservation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reservation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservation\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-purchase-offering-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PurchaseOfferingResponse
---
