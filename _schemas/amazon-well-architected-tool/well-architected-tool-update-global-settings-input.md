---
description: UpdateGlobalSettingsInput schema from AWS Well-Architected Tool API
layout: schema
name: UpdateGlobalSettingsInput
properties_list:
- description: ''
  name: OrganizationSharingStatus
  type: object
- description: ''
  name: DiscoveryIntegrationStatus
  type: object
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-update-global-settings-input-schema.json
slug: well-architected-tool-update-global-settings-input
source_filename: well-architected-tool-update-global-settings-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"UpdateGlobalSettingsInput\",\n  \"properties\": {\n    \"OrganizationSharingStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationSharingStatus\"\n        },\n        {\n          \"description\": \"The status of organization sharing settings.\"\n        }\n      ]\n    },\n    \"DiscoveryIntegrationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiscoveryIntegrationStatus\"\n        },\n        {\n          \"description\": \"The status of discovery support settings.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-update-global-settings-input-schema.json\",\n  \"description\": \"UpdateGlobalSettingsInput schema from AWS Well-Architected Tool API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-update-global-settings-input-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: UpdateGlobalSettingsInput
---
