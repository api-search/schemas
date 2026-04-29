---
description: An application property. It is a caller defined JSON object that Bitbucket will store and return. The `_attributes` field at its top level can be used to control who is allowed to read and update the property. The keys of the JSON object must match an allowed pattern. For details, see [Application properties](/cloud/bitbucket/application-properties/).
layout: schema
name: application_property
properties_list:
- description: ''
  name: _attributes
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-application_property-schema.json
slug: atlassian-bitbucket-repositories-application_property
source_filename: atlassian-bitbucket-repositories-application_property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"application_property\",\n  \"type\": \"object\",\n  \"description\": \"An application property. It is a caller defined JSON object that Bitbucket will store and return. \\nThe `_attributes` field at its top level can be used to control who is allowed to read and update the property. \\nThe keys of the JSON object must match an allowed pattern. For details, \\nsee [Application properties](/cloud/bitbucket/application-properties/).\\n\",\n  \"properties\": {\n    \"_attributes\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-application_property-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: application_property
---
