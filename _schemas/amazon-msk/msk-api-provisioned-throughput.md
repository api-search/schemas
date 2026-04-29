---
description: <p>Contains information about provisioned throughput for EBS storage volumes attached to kafka broker nodes.</p>
layout: schema
name: ProvisionedThroughput
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: VolumeThroughput
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-provisioned-throughput-schema.json
slug: msk-api-provisioned-throughput
source_filename: msk-api-provisioned-throughput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-provisioned-throughput-schema.json\",\n  \"title\": \"ProvisionedThroughput\",\n  \"description\": \"\\n            <p>Contains information about provisioned throughput for EBS storage volumes attached to kafka broker nodes.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabled\"\n          },\n          \"description\": \"\\n            <p>Provisioned throughput is enabled or not.</p>\"\n        }\n      ]\n    },\n    \"VolumeThroughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumeThroughput\"\n\
  \          },\n          \"description\": \"\\n            <p>Throughput value of the EBS volumes for the data drive on each kafka broker node in MiB per second.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-provisioned-throughput-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ProvisionedThroughput
---
