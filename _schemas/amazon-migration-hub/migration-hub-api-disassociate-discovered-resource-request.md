---
description: DisassociateDiscoveredResourceRequest schema from Amazon Migration Hub API
layout: schema
name: DisassociateDiscoveredResourceRequest
properties_list:
- description: ''
  name: ProgressUpdateStream
  type: object
- description: ''
  name: MigrationTaskName
  type: object
- description: ''
  name: ConfigurationId
  type: object
- description: ''
  name: DryRun
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-disassociate-discovered-resource-request-schema.json
slug: migration-hub-api-disassociate-discovered-resource-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-disassociate-discovered-resource-request-schema.json\",\n  \"title\": \"DisassociateDiscoveredResourceRequest\",\n  \"description\": \"DisassociateDiscoveredResourceRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"The name of the ProgressUpdateStream.\"\n        }\n      ]\n    },\n    \"MigrationTaskName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTaskName\"\n        },\n        {\n          \"description\": \"The identifier given to the MigrationTask. <i>Do not store personal data in this field.</i> \"\n    \
  \    }\n      ]\n    },\n    \"ConfigurationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationId\"\n        },\n        {\n          \"description\": \"ConfigurationId of the Application Discovery Service resource to be disassociated.\"\n        }\n      ]\n    },\n    \"DryRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DryRun\"\n        },\n        {\n          \"description\": \"Optional boolean flag to indicate whether any effect should take place. Used to test if the caller has permission to make the call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ProgressUpdateStream\",\n    \"MigrationTaskName\",\n    \"ConfigurationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-disassociate-discovered-resource-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DisassociateDiscoveredResourceRequest
---
