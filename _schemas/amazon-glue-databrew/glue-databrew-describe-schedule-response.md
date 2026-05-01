---
description: DescribeScheduleResponse schema from Amazon Glue DataBrew API
layout: schema
name: DescribeScheduleResponse
properties_list:
- description: ''
  name: CreateDate
  type: object
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: JobNames
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: CronExpression
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-describe-schedule-response-schema.json
slug: glue-databrew-describe-schedule-response
source_filename: glue-databrew-describe-schedule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-schedule-response-schema.json\",\n  \"title\": \"DescribeScheduleResponse\",\n  \"description\": \"DescribeScheduleResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the schedule was created.\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user who created the schedule. \"\n        }\n      ]\n    },\n    \"JobNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobNameList\"\
  \n        },\n        {\n          \"description\": \"The name or names of one or more jobs to be run by using the schedule.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user who last modified the schedule.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the schedule was last modified.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the schedule.\"\n        }\n      ]\n    },\n    \"CronExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CronExpression\"\
  \n        },\n        {\n          \"description\": \"The date or dates and time or times when the jobs are to be run for the schedule. For more information, see <a href=\\\"https://docs.aws.amazon.com/databrew/latest/dg/jobs.cron.html\\\">Cron expressions</a> in the <i>Glue DataBrew Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags associated with this schedule.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleName\"\n        },\n        {\n          \"description\": \"The name of the schedule.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-schedule-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DescribeScheduleResponse
---
