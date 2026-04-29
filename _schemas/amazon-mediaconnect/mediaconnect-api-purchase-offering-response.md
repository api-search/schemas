---
description: PurchaseOfferingResponse schema from AWS Elemental MediaConnect API
layout: schema
name: PurchaseOfferingResponse
properties_list:
- description: ''
  name: Reservation
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-purchase-offering-response-schema.json
slug: mediaconnect-api-purchase-offering-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-purchase-offering-response-schema.json\",\n  \"title\": \"PurchaseOfferingResponse\",\n  \"description\": \"PurchaseOfferingResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Reservation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reservation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservation\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-purchase-offering-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: PurchaseOfferingResponse
---
