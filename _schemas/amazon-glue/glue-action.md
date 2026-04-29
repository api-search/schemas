---
description: Defines an action to be initiated by a trigger.
layout: schema
name: Action
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: Arguments
  type: object
- description: ''
  name: Timeout
  type: object
- description: ''
  name: SecurityConfiguration
  type: object
- description: ''
  name: NotificationProperty
  type: object
- description: ''
  name: CrawlerName
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-action-schema.json
slug: glue-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"Defines an action to be initiated by a trigger.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of a job to be run.\"\n        }\n      ]\n    },\n    \"Arguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericMap\"\n        },\n        {\n          \"description\": \"<p>The job arguments used when this trigger fires. For this job run, they replace the default arguments set in the job definition itself.</p> <p>You can specify arguments here that your own job-execution script consumes, as well as arguments that Glue itself consumes.</p>\
  \ <p>For information about how to specify and consume your own Job arguments, see the <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-python-calling.html\\\">Calling Glue APIs in Python</a> topic in the developer guide.</p> <p>For information about the key-value pairs that Glue consumes to set up your job, see the <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-glue-arguments.html\\\">Special Parameters Used by Glue</a> topic in the developer guide.</p>\"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"The <code>JobRun</code> timeout in minutes. This is the maximum time that a job run can consume resources before it is terminated and enters <code>TIMEOUT</code> status. The default is 2,880 minutes (48 hours). This overrides the timeout value set in the parent job.\"\n        }\n      ]\n   \
  \ },\n    \"SecurityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the <code>SecurityConfiguration</code> structure to be used with this action.\"\n        }\n      ]\n    },\n    \"NotificationProperty\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationProperty\"\n        },\n        {\n          \"description\": \"Specifies configuration properties of a job run notification.\"\n        }\n      ]\n    },\n    \"CrawlerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the crawler to be used with this action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-action-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: Action
---
