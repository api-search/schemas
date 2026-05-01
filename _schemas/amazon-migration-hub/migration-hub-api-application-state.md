---
description: The state of an application discovered through Migration Hub import, the AWS Agentless Discovery Connector, or the AWS Application Discovery Agent.
layout: schema
name: ApplicationState
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: ApplicationStatus
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-application-state-schema.json
slug: migration-hub-api-application-state
source_filename: migration-hub-api-application-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-application-state-schema.json\",\n  \"title\": \"ApplicationState\",\n  \"description\": \"The state of an application discovered through Migration Hub import, the AWS Agentless Discovery Connector, or the AWS Application Discovery Agent.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationId\"\n        },\n        {\n          \"description\": \"The configurationId from the Application Discovery Service that uniquely identifies an application.\"\n        }\n      ]\n    },\n    \"ApplicationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationStatus\"\n        },\n        {\n          \"description\": \"The current status of an\
  \ application.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateDateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the application status was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-application-state-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ApplicationState
---
