---
description: A structure that can contain a value in multiple encoding formats.
layout: schema
name: ValueHolder
properties_list:
- description: ''
  name: IonText
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-value-holder-schema.json
slug: amazon-qldb-value-holder
source_filename: amazon-qldb-value-holder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-value-holder-schema.json\",\n  \"title\": \"ValueHolder\",\n  \"description\": \"A structure that can contain a value in multiple encoding formats.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IonText\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IonText\"\n        },\n        {\n          \"description\": \"An Amazon Ion plaintext value contained in a <code>ValueHolder</code> structure.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-value-holder-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: ValueHolder
---
