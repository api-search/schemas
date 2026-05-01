---
description: Reboots a node.
layout: schema
name: RebootBrokerRequest
properties_list:
- description: ''
  name: BrokerIds
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-reboot-broker-request-schema.json
slug: msk-api-reboot-broker-request
source_filename: msk-api-reboot-broker-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-reboot-broker-request-schema.json\",\n  \"title\": \"RebootBrokerRequest\",\n  \"description\": \"Reboots a node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerIds\"\n          },\n          \"description\": \"\\n            <p>The list of broker IDs to be rebooted. The reboot-broker operation supports rebooting one broker at a time.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BrokerIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-reboot-broker-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: RebootBrokerRequest
---
