---
description: DescribeOfferingResponse schema from AWS Elemental MediaConnect API
layout: schema
name: DescribeOfferingResponse
properties_list:
- description: ''
  name: Offering
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-describe-offering-response-schema.json
slug: mediaconnect-api-describe-offering-response
source_filename: mediaconnect-api-describe-offering-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-describe-offering-response-schema.json\",\n  \"title\": \"DescribeOfferingResponse\",\n  \"description\": \"DescribeOfferingResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Offering\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Offering\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offering\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-describe-offering-response-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: DescribeOfferingResponse
---
