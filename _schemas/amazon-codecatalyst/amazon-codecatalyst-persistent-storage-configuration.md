---
description: Information about the configuration of persistent storage for a Dev Environment.
layout: schema
name: PersistentStorageConfiguration
properties_list:
- description: ''
  name: sizeInGiB
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-persistent-storage-configuration-schema.json
slug: amazon-codecatalyst-persistent-storage-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-persistent-storage-configuration-schema.json\",\n  \"title\": \"PersistentStorageConfiguration\",\n  \"description\": \"Information about the configuration of persistent storage for a Dev Environment. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sizeInGiB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PersistentStorageConfigurationSizeInGiBInteger\"\n        },\n        {\n          \"description\": \"<p>The size of the persistent storage in gigabytes (specifically GiB).</p> <note> <p>Valid values for storage are based on memory sizes in 16GB increments. Valid values are 16, 32, and 64.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"sizeInGiB\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-persistent-storage-configuration-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: PersistentStorageConfiguration
---
