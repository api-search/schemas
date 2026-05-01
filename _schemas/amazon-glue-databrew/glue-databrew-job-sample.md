---
description: A sample configuration for profile jobs only, which determines the number of rows on which the profile job is run. If a <code>JobSample</code> value isn't provided, the default is used. The default value is CUSTOM_ROWS for the mode parameter and 20,000 for the size parameter.
layout: schema
name: JobSample
properties_list:
- description: ''
  name: Mode
  type: object
- description: ''
  name: Size
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-job-sample-schema.json
slug: glue-databrew-job-sample
source_filename: glue-databrew-job-sample-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-job-sample-schema.json\",\n  \"title\": \"JobSample\",\n  \"description\": \"A sample configuration for profile jobs only, which determines the number of rows on which the profile job is run. If a <code>JobSample</code> value isn't provided, the default is used. The default value is CUSTOM_ROWS for the mode parameter and 20,000 for the size parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SampleMode\"\n        },\n        {\n          \"description\": \"<p>A value that determines whether the profile job is run on the entire dataset or a specified number of rows. This value must be one of the following:</p> <ul> <li> <p>FULL_DATASET - The profile job is run on the entire dataset.</p>\
  \ </li> <li> <p>CUSTOM_ROWS - The profile job is run on the number of rows specified in the <code>Size</code> parameter.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Size\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobSize\"\n        },\n        {\n          \"description\": \"<p>The <code>Size</code> parameter is only required when the mode is CUSTOM_ROWS. The profile job is run on the specified number of rows. The maximum value for size is Long.MAX_VALUE.</p> <p>Long.MAX_VALUE = 9223372036854775807</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-job-sample-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: JobSample
---
