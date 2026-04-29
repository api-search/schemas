---
description: <p>A user-defined key-value pair that describes metadata added to an DMS resource and that is used by operations such as the following:</p> <ul> <li> <p> <code>AddTagsToResource</code> </p> </li> <li> <p> <code>ListTagsForResource</code> </p> </li> <li> <p> <code>RemoveTagsFromResource</code> </p> </li> </ul>
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-tag-schema.json
slug: amazon-dms-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"<p>A user-defined key-value pair that describes metadata added to an DMS resource and that is used by operations such as the following:</p> <ul> <li> <p> <code>AddTagsToResource</code> </p> </li> <li> <p> <code>ListTagsForResource</code> </p> </li> <li> <p> <code>RemoveTagsFromResource</code> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A key is the required name of the tag. The string value can be 1-128 Unicode characters in length and can't be prefixed with \\\"aws:\\\" or \\\"dms:\\\". The string can only contain only the set of Unicode letters, digits, white-space,\
  \ '_', '.', '/', '=', '+', '-' (Java regular expressions: \\\"^([\\\\\\\\p{L}\\\\\\\\p{Z}\\\\\\\\p{N}_.:/=+\\\\\\\\-]*)$\\\").\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A value is the optional value of the tag. The string value can be 1-256 Unicode characters in length and can't be prefixed with \\\"aws:\\\" or \\\"dms:\\\". The string can only contain only the set of Unicode letters, digits, white-space, '_', '.', '/', '=', '+', '-' (Java regular expressions: \\\"^([\\\\\\\\p{L}\\\\\\\\p{Z}\\\\\\\\p{N}_.:/=+\\\\\\\\-]*)$\\\").\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) string that uniquely identifies the resource for which the tag is created.\"\n        }\n      ]\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-tag-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: Tag
---
