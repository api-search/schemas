---
description: PutResourceAttributesRequest schema from Amazon Migration Hub API
layout: schema
name: PutResourceAttributesRequest
properties_list:
- description: ''
  name: ProgressUpdateStream
  type: object
- description: ''
  name: MigrationTaskName
  type: object
- description: ''
  name: ResourceAttributeList
  type: object
- description: ''
  name: DryRun
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-put-resource-attributes-request-schema.json
slug: migration-hub-api-put-resource-attributes-request
source_filename: migration-hub-api-put-resource-attributes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-put-resource-attributes-request-schema.json\",\n  \"title\": \"PutResourceAttributesRequest\",\n  \"description\": \"PutResourceAttributesRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"The name of the ProgressUpdateStream. \"\n        }\n      ]\n    },\n    \"MigrationTaskName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTaskName\"\n        },\n        {\n          \"description\": \"Unique identifier that references the migration task. <i>Do not store personal data in this field.</i> \"\n        }\n      ]\n\
  \    },\n    \"ResourceAttributeList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceAttributeList\"\n        },\n        {\n          \"description\": \"<p>Information about the resource that is being migrated. This data will be used to map the task to a resource in the Application Discovery Service repository.</p> <note> <p>Takes the object array of <code>ResourceAttribute</code> where the <code>Type</code> field is reserved for the following values: <code>IPV4_ADDRESS | IPV6_ADDRESS | MAC_ADDRESS | FQDN | VM_MANAGER_ID | VM_MANAGED_OBJECT_REFERENCE | VM_NAME | VM_PATH | BIOS_ID | MOTHERBOARD_SERIAL_NUMBER</code> where the identifying value can be a string up to 256 characters.</p> </note> <important> <ul> <li> <p>If any \\\"VM\\\" related value is set for a <code>ResourceAttribute</code> object, it is required that <code>VM_MANAGER_ID</code>, as a minimum, is always set. If <code>VM_MANAGER_ID</code> is not set, then all \\\"VM\\\" fields will\
  \ be discarded and \\\"VM\\\" fields will not be used for matching the migration task to a server in Application Discovery Service repository. See the <a href=\\\"https://docs.aws.amazon.com/migrationhub/latest/ug/API_PutResourceAttributes.html#API_PutResourceAttributes_Examples\\\">Example</a> section below for a use case of specifying \\\"VM\\\" related values.</p> </li> <li> <p> If a server you are trying to match has multiple IP or MAC addresses, you should provide as many as you know in separate type/value pairs passed to the <code>ResourceAttributeList</code> parameter to maximize the chances of matching.</p> </li> </ul> </important>\"\n        }\n      ]\n    },\n    \"DryRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DryRun\"\n        },\n        {\n          \"description\": \"Optional boolean flag to indicate whether any effect should take place. Used to test if the caller has permission to make the call.\"\n        }\n      ]\n    }\n  },\n\
  \  \"required\": [\n    \"ProgressUpdateStream\",\n    \"MigrationTaskName\",\n    \"ResourceAttributeList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-put-resource-attributes-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PutResourceAttributesRequest
---
