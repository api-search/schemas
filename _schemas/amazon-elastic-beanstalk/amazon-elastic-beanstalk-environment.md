---
description: Schema representing an AWS Elastic Beanstalk environment, which is a collection of AWS resources running an application version deployed on a specific platform.
layout: schema
name: AWS Elastic Beanstalk Environment
properties_list:
- description: The ID of this environment.
  name: EnvironmentId
  type: string
- description: The name of this environment.
  name: EnvironmentName
  type: string
- description: The ARN of this environment.
  name: EnvironmentArn
  type: string
- description: The name of the application associated with this environment.
  name: ApplicationName
  type: string
- description: The application version deployed in this running environment.
  name: VersionLabel
  type:
  - string
  - 'null'
- description: The name of the SolutionStack deployed with this environment.
  name: SolutionStackName
  type:
  - string
  - 'null'
- description: The ARN of the platform version.
  name: PlatformArn
  type:
  - string
  - 'null'
- description: The name of the configuration template used to originally launch this environment.
  name: TemplateName
  type:
  - string
  - 'null'
- description: Describes this environment.
  name: Description
  type:
  - string
  - 'null'
- description: For load-balanced, autoscaling environments, the URL to the LoadBalancer.
  name: EndpointURL
  type:
  - string
  - 'null'
- description: The URL to the CNAME for this environment.
  name: CNAME
  type:
  - string
  - 'null'
- description: The creation date for this environment.
  name: DateCreated
  type: string
- description: The last modified date for this environment.
  name: DateUpdated
  type: string
- description: The current operational status of the environment.
  name: Status
  type: string
- description: Indicates if there is an in-progress environment configuration update or application version deployment that you can cancel.
  name: AbortableOperationInProgress
  type: boolean
- description: Describes the health status of the environment.
  name: Health
  type: string
- description: Returns the health status of the application running in your environment.
  name: HealthStatus
  type: string
- description: Describes the current tier of this environment.
  name: Tier
  type: object
- description: The description of the AWS resources used by this environment.
  name: Resources
  type: object
- description: A list of links to other environments in the same group.
  name: EnvironmentLinks
  type: array
- description: The Amazon Resource Name (ARN) of the environment's operations role.
  name: OperationsRole
  type:
  - string
  - 'null'
provider_name: Amazon Elastic Beanstalk
provider_slug: amazon-elastic-beanstalk
schema_file: json-schema/amazon-elastic-beanstalk-environment-schema.json
slug: amazon-elastic-beanstalk-environment
source_filename: amazon-elastic-beanstalk-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apis.io/schemas/amazon-elastic-beanstalk-environment.json\",\n  \"title\": \"AWS Elastic Beanstalk Environment\",\n  \"description\": \"Schema representing an AWS Elastic Beanstalk environment, which is a collection of AWS resources running an application version deployed on a specific platform.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ApplicationName\"\n  ],\n  \"properties\": {\n    \"EnvironmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of this environment.\",\n      \"pattern\": \"^e-[a-z0-9]+$\"\n    },\n    \"EnvironmentName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of this environment.\",\n      \"minLength\": 4,\n      \"maxLength\": 40\n    },\n    \"EnvironmentArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of this environment.\",\n      \"pattern\": \"^arn:aws[a-zA-Z-]*:elasticbeanstalk:[a-z0-9-]+:[0-9]{12}:environment/.+/.+$\"\
  \n    },\n    \"ApplicationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application associated with this environment.\",\n      \"minLength\": 1,\n      \"maxLength\": 100\n    },\n    \"VersionLabel\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The application version deployed in this running environment.\"\n    },\n    \"SolutionStackName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the SolutionStack deployed with this environment.\"\n    },\n    \"PlatformArn\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ARN of the platform version.\"\n    },\n    \"TemplateName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of the configuration template used to originally launch this environment.\"\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Describes this environment.\",\n      \"\
  maxLength\": 200\n    },\n    \"EndpointURL\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"For load-balanced, autoscaling environments, the URL to the LoadBalancer.\"\n    },\n    \"CNAME\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The URL to the CNAME for this environment.\"\n    },\n    \"DateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation date for this environment.\"\n    },\n    \"DateUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last modified date for this environment.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current operational status of the environment.\",\n      \"enum\": [\n        \"Aborting\",\n        \"Launching\",\n        \"Updating\",\n        \"LinkingFrom\",\n        \"LinkingTo\",\n        \"Ready\",\n        \"Terminating\",\n        \"Terminated\"\
  \n      ]\n    },\n    \"AbortableOperationInProgress\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if there is an in-progress environment configuration update or application version deployment that you can cancel.\"\n    },\n    \"Health\": {\n      \"type\": \"string\",\n      \"description\": \"Describes the health status of the environment.\",\n      \"enum\": [\n        \"Green\",\n        \"Yellow\",\n        \"Red\",\n        \"Grey\"\n      ]\n    },\n    \"HealthStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Returns the health status of the application running in your environment.\",\n      \"enum\": [\n        \"NoData\",\n        \"Unknown\",\n        \"Pending\",\n        \"Ok\",\n        \"Info\",\n        \"Warning\",\n        \"Degraded\",\n        \"Severe\",\n        \"Suspended\"\n      ]\n    },\n    \"Tier\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the current tier of this environment.\",\n    \
  \  \"properties\": {\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of this environment tier.\",\n          \"enum\": [\n            \"WebServer\",\n            \"Worker\"\n          ]\n        },\n        \"Type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of this environment tier.\",\n          \"enum\": [\n            \"Standard\",\n            \"SQS/HTTP\"\n          ]\n        },\n        \"Version\": {\n          \"type\": \"string\",\n          \"description\": \"The version of this environment tier.\"\n        }\n      }\n    },\n    \"Resources\": {\n      \"type\": \"object\",\n      \"description\": \"The description of the AWS resources used by this environment.\",\n      \"properties\": {\n        \"LoadBalancer\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"LoadBalancerName\": {\n              \"type\": \"string\",\n              \"description\": \"The name of\
  \ the LoadBalancer.\"\n            },\n            \"Domain\": {\n              \"type\": \"string\",\n              \"description\": \"The domain name of the LoadBalancer.\"\n            },\n            \"Listeners\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"Protocol\": {\n                    \"type\": \"string\"\n                  },\n                  \"Port\": {\n                    \"type\": \"integer\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"EnvironmentLinks\": {\n      \"type\": \"array\",\n      \"description\": \"A list of links to other environments in the same group.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"LinkName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the link.\"\n          },\n\
  \          \"EnvironmentName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the linked environment.\"\n          }\n        }\n      }\n    },\n    \"OperationsRole\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The Amazon Resource Name (ARN) of the environment's operations role.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-beanstalk/refs/heads/main/json-schema/amazon-elastic-beanstalk-environment-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Deployment
- Elastic Beanstalk
- PaaS
- Platform As A Service
- Web Applications
title: AWS Elastic Beanstalk Environment
---
