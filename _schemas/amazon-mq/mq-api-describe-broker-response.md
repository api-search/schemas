---
description: DescribeBrokerResponse schema from Amazon MQ API
layout: schema
name: DescribeBrokerResponse
properties_list:
- description: ''
  name: ActionsRequired
  type: object
- description: ''
  name: AuthenticationStrategy
  type: object
- description: ''
  name: AutoMinorVersionUpgrade
  type: object
- description: ''
  name: BrokerArn
  type: object
- description: ''
  name: BrokerId
  type: object
- description: ''
  name: BrokerInstances
  type: object
- description: ''
  name: BrokerName
  type: object
- description: ''
  name: BrokerState
  type: object
- description: ''
  name: Configurations
  type: object
- description: ''
  name: Created
  type: object
- description: ''
  name: DeploymentMode
  type: object
- description: ''
  name: EncryptionOptions
  type: object
- description: ''
  name: EngineType
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
  name: PendingAuthenticationStrategy
  type: object
- description: ''
  name: PendingEngineVersion
  type: object
- description: ''
  name: PendingHostInstanceType
  type: object
- description: ''
  name: PendingLdapServerMetadata
  type: object
- description: ''
  name: PendingSecurityGroups
  type: object
- description: ''
  name: PubliclyAccessible
  type: object
- description: ''
  name: SecurityGroups
  type: object
- description: ''
  name: StorageType
  type: object
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Users
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-describe-broker-response-schema.json
slug: mq-api-describe-broker-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-describe-broker-response-schema.json\",\n  \"title\": \"DescribeBrokerResponse\",\n  \"description\": \"DescribeBrokerResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionsRequired\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfActionRequired\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"actionsRequired\"\n          },\n          \"description\": \"A list of actions required for a broker.\"\n        }\n      ]\n    },\n    \"AuthenticationStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationStrategy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"authenticationStrategy\"\n          },\n          \"description\": \"The authentication\
  \ strategy used to secure the broker. The default is SIMPLE.\"\n        }\n      ]\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoMinorVersionUpgrade\"\n          },\n          \"description\": \"Enables automatic upgrades to new minor versions for brokers, as new versions are released and supported by Amazon MQ. Automatic upgrades occur during the scheduled maintenance window of the broker or after a manual broker reboot.\"\n        }\n      ]\n    },\n    \"BrokerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerArn\"\n          },\n          \"description\": \"The broker's Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"BrokerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerId\"\n          },\n          \"description\": \"The unique ID that Amazon MQ generates for the broker.\"\n        }\n      ]\n    },\n    \"BrokerInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBrokerInstance\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerInstances\"\n          },\n          \"description\": \"A list of information about allocated brokers.\"\n        }\n      ]\n    },\n    \"BrokerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerName\"\n          },\n          \"description\": \"The broker's name. This value must be unique in your AWS account, 1-50 characters long, must contain only letters, numbers, dashes, and underscores, and must not contain white spaces, brackets, wildcard characters, or\
  \ special characters.\"\n        }\n      ]\n    },\n    \"BrokerState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerState\"\n          },\n          \"description\": \"The broker's status.\"\n        }\n      ]\n    },\n    \"Configurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Configurations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurations\"\n          },\n          \"description\": \"The list of all revisions for the specified configuration.\"\n        }\n      ]\n    },\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"created\"\n          },\n          \"description\": \"The time when the broker was created.\"\n        }\n      ]\n    },\n    \"DeploymentMode\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deploymentMode\"\n          },\n          \"description\": \"The broker's deployment mode.\"\n        }\n      ]\n    },\n    \"EncryptionOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionOptions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionOptions\"\n          },\n          \"description\": \"Encryption options for the broker. Does not apply to RabbitMQ brokers.\"\n        }\n      ]\n    },\n    \"EngineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineType\"\n          },\n          \"description\": \"The type of broker engine. Currently, Amazon MQ supports ACTIVEMQ and RABBITMQ.\"\n        }\n      ]\n    },\n   \
  \ \"EngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineVersion\"\n          },\n          \"description\": \"The broker engine's version. For a list of supported engine versions, see <a href=\\\"https://docs.aws.amazon.com//amazon-mq/latest/developer-guide/broker-engine.html\\\">Supported engines</a>.\"\n        }\n      ]\n    },\n    \"HostInstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hostInstanceType\"\n          },\n          \"description\": \"The broker's instance type.\"\n        }\n      ]\n    },\n    \"LdapServerMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LdapServerMetadataOutput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ldapServerMetadata\"\n     \
  \     },\n          \"description\": \"The metadata of the LDAP server used to authenticate and authorize connections to the broker.\"\n        }\n      ]\n    },\n    \"Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogsSummary\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logs\"\n          },\n          \"description\": \"The list of information about logs currently enabled and pending to be deployed for the specified broker.\"\n        }\n      ]\n    },\n    \"MaintenanceWindowStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WeeklyStartTime\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceWindowStartTime\"\n          },\n          \"description\": \"The parameters that determine the WeeklyStartTime.\"\n        }\n      ]\n    },\n    \"PendingAuthenticationStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationStrategy\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"pendingAuthenticationStrategy\"\n          },\n          \"description\": \"The authentication strategy that will be applied when the broker is rebooted. The default is SIMPLE.\"\n        }\n      ]\n    },\n    \"PendingEngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pendingEngineVersion\"\n          },\n          \"description\": \"The broker engine version to upgrade to. For a list of supported engine versions, see <a href=\\\"https://docs.aws.amazon.com//amazon-mq/latest/developer-guide/broker-engine.html\\\">Supported engines</a>.\"\n        }\n      ]\n    },\n    \"PendingHostInstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pendingHostInstanceType\"\n          },\n\
  \          \"description\": \"The broker's host instance type to upgrade to. For a list of supported instance types, see <a href=\\\"https://docs.aws.amazon.com//amazon-mq/latest/developer-guide/broker.html#broker-instance-types\\\">Broker instance types</a>.\"\n        }\n      ]\n    },\n    \"PendingLdapServerMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LdapServerMetadataOutput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pendingLdapServerMetadata\"\n          },\n          \"description\": \"The metadata of the LDAP server that will be used to authenticate and authorize connections to the broker after it is rebooted.\"\n        }\n      ]\n    },\n    \"PendingSecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pendingSecurityGroups\"\n          },\n          \"description\": \"The\
  \ list of pending security groups to authorize connections to brokers.\"\n        }\n      ]\n    },\n    \"PubliclyAccessible\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"publiclyAccessible\"\n          },\n          \"description\": \"Enables connections from applications outside of the VPC that hosts the broker's subnets.\"\n        }\n      ]\n    },\n    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroups\"\n          },\n          \"description\": \"The list of rules (1 minimum, 125 maximum) that authorize connections to brokers.\"\n        }\n      ]\n    },\n    \"StorageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerStorageType\"\n        },\n        {\n          \"xml\":\
  \ {\n            \"name\": \"storageType\"\n          },\n          \"description\": \"The broker's storage type.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetIds\"\n          },\n          \"description\": \"The list of groups that define which subnets and IP ranges the broker can use from different Availability Zones.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The list of all tags associated with this broker.\"\n        }\n      ]\n    },\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUserSummary\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"users\"\n          },\n          \"description\": \"The list of all broker usernames for the specified broker.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-describe-broker-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeBrokerResponse
---
