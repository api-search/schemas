---
description: Represents additional options for correct interpretation of datetime parameters used in the Amazon S3 path of a dataset.
layout: schema
name: DatetimeOptions
properties_list:
- description: ''
  name: Format
  type: object
- description: ''
  name: TimezoneOffset
  type: object
- description: ''
  name: LocaleCode
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-datetime-options-schema.json
slug: glue-databrew-datetime-options
source_filename: glue-databrew-datetime-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-datetime-options-schema.json\",\n  \"title\": \"DatetimeOptions\",\n  \"description\": \"Represents additional options for correct interpretation of datetime parameters used in the Amazon S3 path of a dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatetimeFormat\"\n        },\n        {\n          \"description\": \"Required option, that defines the datetime format used for a date parameter in the Amazon S3 path. Should use only supported datetime specifiers and separation characters, all literal a-z or A-Z characters should be escaped with single quotes. E.g. \\\"MM.dd.yyyy-'at'-HH:mm\\\".\"\n        }\n      ]\n    },\n    \"TimezoneOffset\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/TimezoneOffset\"\n        },\n        {\n          \"description\": \"Optional value for a timezone offset of the datetime parameter value in the Amazon S3 path. Shouldn't be used if Format for this parameter includes timezone fields. If no offset specified, UTC is assumed.\"\n        }\n      ]\n    },\n    \"LocaleCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocaleCode\"\n        },\n        {\n          \"description\": \"Optional value for a non-US locale code, needed for correct interpretation of some date formats.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Format\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-datetime-options-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DatetimeOptions
---
