---
description: An ARN of the AWS cloud resource target receiving the migration (e.g., AMI, EC2 instance, RDS instance, etc.).
layout: schema
name: CreatedArtifact
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-created-artifact-schema.json
slug: migration-hub-api-created-artifact
source_filename: migration-hub-api-created-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-created-artifact-schema.json\",\n  \"title\": \"CreatedArtifact\",\n  \"description\": \"An ARN of the AWS cloud resource target receiving the migration (e.g., AMI, EC2 instance, RDS instance, etc.).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedArtifactName\"\n        },\n        {\n          \"description\": \"An ARN that uniquely identifies the result of a migration task.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedArtifactDescription\"\n        },\n        {\n          \"description\": \"A description that can be free-form text to record additional detail about the artifact for clarity\
  \ or for later reference.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-created-artifact-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreatedArtifact
---
