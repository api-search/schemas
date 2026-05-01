---
description: Represents the data being transformed during an action.
layout: schema
name: ViewFrame
properties_list:
- description: ''
  name: StartColumnIndex
  type: object
- description: ''
  name: ColumnRange
  type: object
- description: ''
  name: HiddenColumns
  type: object
- description: ''
  name: StartRowIndex
  type: object
- description: ''
  name: RowRange
  type: object
- description: ''
  name: Analytics
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-view-frame-schema.json
slug: glue-databrew-view-frame
source_filename: glue-databrew-view-frame-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-view-frame-schema.json\",\n  \"title\": \"ViewFrame\",\n  \"description\": \"Represents the data being transformed during an action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartColumnIndex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartColumnIndex\"\n        },\n        {\n          \"description\": \"The starting index for the range of columns to return in the view frame.\"\n        }\n      ]\n    },\n    \"ColumnRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnRange\"\n        },\n        {\n          \"description\": \"The number of columns to include in the view frame, beginning with the <code>StartColumnIndex</code> value and ignoring any columns in the <code>HiddenColumns</code> list.\"\
  \n        }\n      ]\n    },\n    \"HiddenColumns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HiddenColumnList\"\n        },\n        {\n          \"description\": \"A list of columns to hide in the view frame.\"\n        }\n      ]\n    },\n    \"StartRowIndex\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartRowIndex\"\n        },\n        {\n          \"description\": \"The starting index for the range of rows to return in the view frame.\"\n        }\n      ]\n    },\n    \"RowRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RowRange\"\n        },\n        {\n          \"description\": \"The number of rows to include in the view frame, beginning with the <code>StartRowIndex</code> value.\"\n        }\n      ]\n    },\n    \"Analytics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalyticsMode\"\n        },\n        {\n          \"description\"\
  : \"Controls if analytics computation is enabled or disabled. Enabled by default.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StartColumnIndex\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-view-frame-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ViewFrame
---
