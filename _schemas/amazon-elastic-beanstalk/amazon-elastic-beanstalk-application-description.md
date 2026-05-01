---
description: ApplicationDescription schema from Amazon Elastic Beanstalk AWS Elastic Beanstalk API
layout: schema
name: ApplicationDescription
properties_list:
- description: The Amazon Resource Name (ARN) of the application.
  name: ApplicationArn
  type: string
- description: The name of the application.
  name: ApplicationName
  type: string
- description: User-defined description of the application.
  name: Description
  type: string
- description: The date when the application was created.
  name: DateCreated
  type: string
- description: The date when the application was last modified.
  name: DateUpdated
  type: string
- description: The names of the versions for this application.
  name: Versions
  type: array
- description: The names of the configuration templates associated with this application.
  name: ConfigurationTemplates
  type: array
- description: The lifecycle settings for the application.
  name: ResourceLifecycleConfig
  type: object
provider_name: Amazon Elastic Beanstalk
provider_slug: amazon-elastic-beanstalk
schema_file: json-schema/amazon-elastic-beanstalk-application-description-schema.json
slug: amazon-elastic-beanstalk-application-description
source_filename: amazon-elastic-beanstalk-application-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/json-schema/amazon-elastic-beanstalk-application-description-schema.json\",\n  \"title\": \"ApplicationDescription\",\n  \"description\": \"ApplicationDescription schema from Amazon Elastic Beanstalk AWS Elastic Beanstalk API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the application.\"\n    },\n    \"ApplicationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined description of the application.\"\n    },\n    \"DateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date when the application\
  \ was created.\"\n    },\n    \"DateUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date when the application was last modified.\"\n    },\n    \"Versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The names of the versions for this application.\"\n    },\n    \"ConfigurationTemplates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The names of the configuration templates associated with this application.\"\n    },\n    \"ResourceLifecycleConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ServiceRole\": {\n          \"type\": \"string\"\n        },\n        \"VersionLifecycleConfig\": {\n          \"type\": \"object\"\n        }\n      },\n      \"description\": \"The lifecycle settings for the application.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/json-schema/amazon-elastic-beanstalk-application-description-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Deployment
- Elastic Beanstalk
- PaaS
- Platform As A Service
- Web Applications
title: ApplicationDescription
---
