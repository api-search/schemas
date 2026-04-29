---
description: ListProvisioningTemplateVersionsResponse schema
layout: schema
name: ListProvisioningTemplateVersionsResponse
properties_list:
- description: ''
  name: versions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-list-provisioning-template-versions-response-schema.json
slug: iot-device-defender-list-provisioning-template-versions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-provisioning-template-versions-response-schema.json\",\n  \"title\": \"ListProvisioningTemplateVersionsResponse\",\n  \"description\": \"ListProvisioningTemplateVersionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisioningTemplateVersionListing\"\n        },\n        {\n          \"description\": \"The list of provisioning template versions.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token to retrieve the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-list-provisioning-template-versions-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: ListProvisioningTemplateVersionsResponse
---
