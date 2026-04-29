---
description: UpdateBrokerResponse schema from Amazon MQ API
layout: schema
name: UpdateBrokerResponse
properties_list:
- description: ''
  name: AuthenticationStrategy
  type: object
- description: ''
  name: AutoMinorVersionUpgrade
  type: object
- description: ''
  name: BrokerId
  type: object
- description: ''
  name: Configuration
  type: object
- description: ''
  name: EngineVersion
  type: object
- description: ''
  name: HostInstanceType
  type: object
- description: ''
  name: LdapServerMetadata
  type: object
- description: ''
  name: Logs
  type: object
- description: ''
  name: MaintenanceWindowStartTime
  type: object
- description: ''
  name: SecurityGroups
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-update-broker-response-schema.json
slug: mq-api-update-broker-response
source_filename: mq-api-update-broker-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-update-broker-response-schema.json\",\n  \"title\": \"UpdateBrokerResponse\",\n  \"description\": \"UpdateBrokerResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthenticationStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationStrategy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"authenticationStrategy\"\n          },\n          \"description\": \"Optional. The authentication strategy used to secure the broker. The default is SIMPLE.\"\n        }\n      ]\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoMinorVersionUpgrade\"\n   \
  \       },\n          \"description\": \"The new boolean value that specifies whether broker engines automatically upgrade to new minor versions as new versions are released and supported by Amazon MQ.\"\n        }\n      ]\n    },\n    \"BrokerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerId\"\n          },\n          \"description\": \"Required. The unique ID that Amazon MQ generates for the broker.\"\n        }\n      ]\n    },\n    \"Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configuration\"\n          },\n          \"description\": \"The ID of the updated configuration.\"\n        }\n      ]\n    },\n    \"EngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"engineVersion\"\n          },\n          \"description\": \"The broker engine version to upgrade to. For a list of supported engine versions, see <a href=\\\"https://docs.aws.amazon.com//amazon-mq/latest/developer-guide/broker-engine.html\\\">Supported engines</a>.\"\n        }\n      ]\n    },\n    \"HostInstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hostInstanceType\"\n          },\n          \"description\": \"The broker's host instance type to upgrade to. For a list of supported instance types, see <a href=\\\"https://docs.aws.amazon.com//amazon-mq/latest/developer-guide/broker.html#broker-instance-types\\\">Broker instance types</a>.\"\n        }\n      ]\n    },\n    \"LdapServerMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LdapServerMetadataOutput\"\n   \
  \     },\n        {\n          \"xml\": {\n            \"name\": \"ldapServerMetadata\"\n          },\n          \"description\": \"Optional. The metadata of the LDAP server used to authenticate and authorize connections to the broker. Does not apply to RabbitMQ brokers.\"\n        }\n      ]\n    },\n    \"Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Logs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logs\"\n          },\n          \"description\": \"The list of information about logs to be enabled for the specified broker.\"\n        }\n      ]\n    },\n    \"MaintenanceWindowStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WeeklyStartTime\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceWindowStartTime\"\n          },\n          \"description\": \"The parameters that determine the WeeklyStartTime.\"\n        }\n      ]\n    },\n    \"SecurityGroups\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroups\"\n          },\n          \"description\": \"The list of security groups (1 minimum, 5 maximum) that authorizes connections to brokers.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-update-broker-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateBrokerResponse
---
