---
description: Describes the application, including the application Amazon Resource Name (ARN), status, latest version, and input and output configurations.
layout: schema
name: ApplicationDetail
properties_list:
- description: ''
  name: ApplicationARN
  type: object
- description: ''
  name: ApplicationDescription
  type: object
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: RuntimeEnvironment
  type: object
- description: ''
  name: ServiceExecutionRole
  type: object
- description: ''
  name: ApplicationStatus
  type: object
- description: ''
  name: ApplicationVersionId
  type: object
- description: ''
  name: CreateTimestamp
  type: object
- description: ''
  name: LastUpdateTimestamp
  type: object
- description: ''
  name: ApplicationConfigurationDescription
  type: object
- description: ''
  name: CloudWatchLoggingOptionDescriptions
  type: object
- description: ''
  name: ApplicationMaintenanceConfigurationDescription
  type: object
- description: ''
  name: ApplicationVersionUpdatedFrom
  type: object
- description: ''
  name: ApplicationVersionRolledBackFrom
  type: object
- description: ''
  name: ConditionalToken
  type: object
- description: ''
  name: ApplicationVersionRolledBackTo
  type: object
- description: ''
  name: ApplicationMode
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-detail-schema.json
slug: amazon-managed-apache-flink-application-detail
source_filename: amazon-managed-apache-flink-application-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-detail-schema.json\",\n  \"title\": \"ApplicationDetail\",\n  \"description\": \"Describes the application, including the application Amazon Resource Name (ARN), status, latest version, and input and output configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The ARN of the application.\"\n        }\n      ]\n    },\n    \"ApplicationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationDescription\"\n        },\n        {\n          \"description\": \"The description of the application.\"\n        }\n      ]\n    },\n    \"\
  ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application.\"\n        }\n      ]\n    },\n    \"RuntimeEnvironment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeEnvironment\"\n        },\n        {\n          \"description\": \"The runtime environment for the application.\"\n        }\n      ]\n    },\n    \"ServiceExecutionRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"Specifies the IAM role that the application uses to access external resources.\"\n        }\n      ]\n    },\n    \"ApplicationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationStatus\"\n        },\n        {\n          \"description\": \"The status of the application.\"\n        }\n      ]\n    },\n\
  \    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"Provides the current application version. Kinesis Data Analytics updates the <code>ApplicationVersionId</code> each time you update the application.\"\n        }\n      ]\n    },\n    \"CreateTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The current timestamp when the application was created.\"\n        }\n      ]\n    },\n    \"LastUpdateTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The current timestamp when the application was last updated.\"\n        }\n      ]\n    },\n    \"ApplicationConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationConfigurationDescription\"\
  \n        },\n        {\n          \"description\": \"Describes details about the application code and starting parameters for a Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"CloudWatchLoggingOptionDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLoggingOptionDescriptions\"\n        },\n        {\n          \"description\": \"Describes the application Amazon CloudWatch logging options.\"\n        }\n      ]\n    },\n    \"ApplicationMaintenanceConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMaintenanceConfigurationDescription\"\n        },\n        {\n          \"description\": \"The details of the maintenance configuration for the application.\"\n        }\n      ]\n    },\n    \"ApplicationVersionUpdatedFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n   \
  \       \"description\": \"The previous application version before the latest application update. <a>RollbackApplication</a> reverts the application to this version.\"\n        }\n      ]\n    },\n    \"ApplicationVersionRolledBackFrom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"If you reverted the application using <a>RollbackApplication</a>, the application version when <code>RollbackApplication</code> was called.\"\n        }\n      ]\n    },\n    \"ConditionalToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConditionalToken\"\n        },\n        {\n          \"description\": \"A value you use to implement strong concurrency for application updates.\"\n        }\n      ]\n    },\n    \"ApplicationVersionRolledBackTo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n    \
  \    {\n          \"description\": \"The version to which you want to roll back the application.\"\n        }\n      ]\n    },\n    \"ApplicationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMode\"\n        },\n        {\n          \"description\": \"To create a Kinesis Data Analytics Studio notebook, you must set the mode to <code>INTERACTIVE</code>. However, for a Kinesis Data Analytics for Apache Flink application, the mode is optional.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationARN\",\n    \"ApplicationName\",\n    \"RuntimeEnvironment\",\n    \"ApplicationStatus\",\n    \"ApplicationVersionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-detail-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationDetail
---
