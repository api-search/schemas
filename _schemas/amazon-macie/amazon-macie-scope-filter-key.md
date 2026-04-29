---
description: 'The property to use in a condition that determines whether an S3 object is included or excluded from a classification job. Valid values are:'
layout: schema
name: ScopeFilterKey
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-scope-filter-key-schema.json
slug: amazon-macie-scope-filter-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-scope-filter-key-schema.json\",\n  \"title\": \"ScopeFilterKey\",\n  \"description\": \"The property to use in a condition that determines whether an S3 object is included or excluded from a classification job. Valid values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"OBJECT_EXTENSION\",\n    \"OBJECT_LAST_MODIFIED_DATE\",\n    \"OBJECT_SIZE\",\n    \"OBJECT_KEY\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-scope-filter-key-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ScopeFilterKey
---
