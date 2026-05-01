---
description: DescribeApplicationStateRequest schema from Amazon Migration Hub API
layout: schema
name: DescribeApplicationStateRequest
properties_list:
- description: ''
  name: ApplicationId
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-describe-application-state-request-schema.json
slug: migration-hub-api-describe-application-state-request
source_filename: migration-hub-api-describe-application-state-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-describe-application-state-request-schema.json\",\n  \"title\": \"DescribeApplicationStateRequest\",\n  \"description\": \"DescribeApplicationStateRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationId\"\n        },\n        {\n          \"description\": \"The configurationId in Application Discovery Service that uniquely identifies the grouped application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-describe-application-state-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeApplicationStateRequest
---
