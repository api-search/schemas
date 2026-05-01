---
description: A policy configures behavior that you allow or disallow for your account. For information about MediaConvert policies, see the user guide at http://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html
layout: schema
name: Policy
properties_list:
- description: ''
  name: HttpInputs
  type: object
- description: ''
  name: HttpsInputs
  type: object
- description: ''
  name: S3Inputs
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-policy-schema.json
slug: mediaconvert-api-policy
source_filename: mediaconvert-api-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"A policy configures behavior that you allow or disallow for your account. For information about MediaConvert policies, see the user guide at http://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HttpInputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputPolicy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"httpInputs\"\n          },\n          \"description\": \"Allow or disallow jobs that specify HTTP inputs.\"\n        }\n      ]\n    },\n    \"HttpsInputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputPolicy\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"httpsInputs\"\n          },\n          \"description\": \"Allow or disallow jobs that specify HTTPS inputs.\"\n        }\n      ]\n    },\n    \"S3Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputPolicy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Inputs\"\n          },\n          \"description\": \"Allow or disallow jobs that specify Amazon S3 inputs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-policy-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Policy
---
