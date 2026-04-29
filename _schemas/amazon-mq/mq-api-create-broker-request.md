---
description: Creates a broker using the specified properties.
layout: schema
name: CreateBrokerRequest
properties_list:
- description: ''
  name: AuthenticationStrategy
  type: object
- description: ''
  name: AutoMinorVersionUpgrade
  type: object
- description: ''
  name: BrokerName
  type: object
- description: ''
  name: Configuration
  type: object
- description: ''
  name: CreatorRequestId
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
schema_file: json-schema/mq-api-create-broker-request-schema.json
slug: mq-api-create-broker-request
source_filename: mq-api-create-broker-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-create-broker-request-schema.json\",\n  \"title\": \"CreateBrokerRequest\",\n  \"description\": \"Creates a broker using the specified properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthenticationStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationStrategy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"authenticationStrategy\"\n          },\n          \"description\": \"Optional. The authentication strategy used to secure the broker. The default is SIMPLE.\"\n        }\n      ]\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoMinorVersionUpgrade\"\n   \
  \       },\n          \"description\": \"Enables automatic upgrades to new minor versions for brokers, as new versions are released and supported by Amazon MQ. Automatic upgrades occur during the scheduled maintenance window of the broker or after a manual broker reboot. Set to true by default, if no value is specified.\"\n        }\n      ]\n    },\n    \"BrokerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerName\"\n          },\n          \"description\": \"Required. The broker's name. This value must be unique in your AWS account, 1-50 characters long, must contain only letters, numbers, dashes, and underscores, and must not contain white spaces, brackets, wildcard characters, or special characters.\"\n        }\n      ]\n    },\n    \"Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationId\"\n        },\n \
  \       {\n          \"xml\": {\n            \"name\": \"configuration\"\n          },\n          \"description\": \"A list of information about the configuration.\"\n        }\n      ]\n    },\n    \"CreatorRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creatorRequestId\"\n          },\n          \"description\": \"The unique ID that the requester receives for the created broker. Amazon MQ passes your ID with the API action. Note: We recommend using a Universally Unique Identifier (UUID) for the creatorRequestId. You may omit the creatorRequestId if your application doesn't require idempotency.\"\n        }\n      ]\n    },\n    \"DeploymentMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deploymentMode\"\n          },\n          \"description\"\
  : \"Required. The broker's deployment mode.\"\n        }\n      ]\n    },\n    \"EncryptionOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionOptions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionOptions\"\n          },\n          \"description\": \"Encryption options for the broker. Does not apply to RabbitMQ brokers.\"\n        }\n      ]\n    },\n    \"EngineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineType\"\n          },\n          \"description\": \"Required. The type of broker engine. Currently, Amazon MQ supports ACTIVEMQ and RABBITMQ.\"\n        }\n      ]\n    },\n    \"EngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineVersion\"\n        \
  \  },\n          \"description\": \"Required. The broker engine's version. For a list of supported engine versions, see <a href=\\\"https://docs.aws.amazon.com//amazon-mq/latest/developer-guide/broker-engine.html\\\">Supported engines</a>.\"\n        }\n      ]\n    },\n    \"HostInstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hostInstanceType\"\n          },\n          \"description\": \"Required. The broker's instance type.\"\n        }\n      ]\n    },\n    \"LdapServerMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LdapServerMetadataInput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ldapServerMetadata\"\n          },\n          \"description\": \"Optional. The metadata of the LDAP server used to authenticate and authorize connections to the broker. Does not apply to RabbitMQ brokers.\"\n   \
  \     }\n      ]\n    },\n    \"Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Logs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"logs\"\n          },\n          \"description\": \"Enables Amazon CloudWatch logging for brokers.\"\n        }\n      ]\n    },\n    \"MaintenanceWindowStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WeeklyStartTime\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maintenanceWindowStartTime\"\n          },\n          \"description\": \"The parameters that determine the WeeklyStartTime.\"\n        }\n      ]\n    },\n    \"PubliclyAccessible\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"publiclyAccessible\"\n          },\n          \"description\": \"Enables connections from applications outside of the VPC that hosts the\
  \ broker's subnets. Set to false by default, if no value is provided.\"\n        }\n      ]\n    },\n    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroups\"\n          },\n          \"description\": \"The list of rules (1 minimum, 125 maximum) that authorize connections to brokers.\"\n        }\n      ]\n    },\n    \"StorageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrokerStorageType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"storageType\"\n          },\n          \"description\": \"The broker's storage type.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetIds\"\n          },\n          \"description\"\
  : \"<p>The list of groups that define which subnets and IP ranges the broker can use from different Availability Zones. If you specify more than one subnet, the subnets must be in different Availability Zones. Amazon MQ will not be able to create VPC endpoints for your broker with multiple subnets in the same Availability Zone. A SINGLE_INSTANCE deployment requires one subnet (for example, the default subnet). An ACTIVE_STANDBY_MULTI_AZ Amazon MQ for ActiveMQ deployment requires two subnets. A CLUSTER_MULTI_AZ Amazon MQ for RabbitMQ deployment has no subnet requirements when deployed with public accessibility. Deployment without public accessibility requires at least one subnet.</p> <important><p>If you specify subnets in a <a href=\\\"https://docs.aws.amazon.com/vpc/latest/userguide/vpc-sharing.html\\\">shared VPC</a> for a RabbitMQ broker, the associated VPC to which the specified subnets belong must be owned by your AWS account. Amazon MQ will not be able to create VPC endpoints in\
  \ VPCs that are not owned by your AWS account.</p></important>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"Create tags when creating the broker.\"\n        }\n      ]\n    },\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfUser\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"users\"\n          },\n          \"description\": \"<p>Required. The list of broker users (persons or applications) who can access queues and topics. This value can contain only alphanumeric characters, dashes, periods, underscores, and tildes (- . _ ~). This value must be 2-100 characters long.</p> <important><title>Amazon MQ for RabbitMQ</title> <p>When you create an Amazon MQ for RabbitMQ broker, one and only one administrative\
  \ user is accepted and created when a broker is first provisioned. All subsequent broker users are created by making RabbitMQ API calls directly to brokers or via the RabbitMQ web console.</p></important>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EngineVersion\",\n    \"HostInstanceType\",\n    \"AutoMinorVersionUpgrade\",\n    \"Users\",\n    \"BrokerName\",\n    \"DeploymentMode\",\n    \"EngineType\",\n    \"PubliclyAccessible\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-create-broker-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateBrokerRequest
---
