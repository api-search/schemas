---
description: '<p>See https://www.ibm.com/docs/en/workload-automation/9.3.0?topic=zos-coding-variables-in-jcl to get details about limits for both keys and values: 8 for keys (variable names), 44 for values (variable values) In addition, keys will be only alphabetic characters and digits, without any space or special characters (dash, underscore, etc ...)</p> <p>Parameter key: the first character must be alphabetic. Can be of up to 8 alphanumeric characters.</p>'
layout: schema
name: BatchParamKey
properties_list: []
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-batch-param-key-schema.json
slug: amazon-mainframe-modernization-batch-param-key
source_filename: amazon-mainframe-modernization-batch-param-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-batch-param-key-schema.json\",\n  \"title\": \"BatchParamKey\",\n  \"description\": \"<p>See https://www.ibm.com/docs/en/workload-automation/9.3.0?topic=zos-coding-variables-in-jcl to get details about limits for both keys and values: 8 for keys (variable names), 44 for values (variable values) In addition, keys will be only alphabetic characters and digits, without any space or special characters (dash, underscore, etc ...)</p> <p>Parameter key: the first character must be alphabetic. Can be of up to 8 alphanumeric characters.</p>\",\n  \"type\": \"string\",\n  \"pattern\": \"^[A-Za-z][A-Za-z0-9]{1,7}$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-batch-param-key-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: BatchParamKey
---
