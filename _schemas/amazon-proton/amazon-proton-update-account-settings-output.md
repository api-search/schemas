---
description: UpdateAccountSettingsOutput schema from Amazon Proton API
layout: schema
name: UpdateAccountSettingsOutput
properties_list:
- description: ''
  name: accountSettings
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-account-settings-output-schema.json
slug: amazon-proton-update-account-settings-output
source_filename: amazon-proton-update-account-settings-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-account-settings-output-schema.json\",\n  \"title\": \"UpdateAccountSettingsOutput\",\n  \"description\": \"UpdateAccountSettingsOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountSettings\"\n        },\n        {\n          \"description\": \"The Proton pipeline service role and repository data shared across the Amazon Web Services account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-account-settings-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateAccountSettingsOutput
---
