---
description: Schema for a Mule application deployed to the Anypoint Platform, including configuration for CloudHub, Runtime Fabric, and hybrid deployment targets.
layout: schema
name: MuleSoft Anypoint Application
properties_list:
- description: Unique domain name for the application, used as the subdomain in the CloudHub URL
  name: domain
  type: string
- description: Full domain including the platform suffix (e.g., myapp.cloudhub.io)
  name: fullDomain
  type: string
- description: Current deployment status of the application
  name: status
  type: string
- description: Human-readable description of the application purpose and functionality
  name: description
  type: string
- description: Unique identifier of the organization that owns this application
  name: organizationId
  type: string
- description: Unique identifier of the environment where this application is deployed
  name: environmentId
  type: string
- description: Cloud region where the application is deployed
  name: region
  type: string
- description: ''
  name: muleVersion
  type: object
- description: ''
  name: workers
  type: object
- description: The target platform for deployment
  name: deploymentTarget
  type: string
- description: Application properties passed as runtime configuration to the Mule runtime
  name: properties
  type: object
- description: List of property keys that are treated as secure and masked in the UI
  name: secureProperties
  type: array
- description: Timestamp of the last application update or redeployment
  name: lastUpdateTime
  type: string
- description: Timestamp when the application was first created
  name: createdAt
  type: string
- description: Name of the deployed application archive file (JAR or ZIP)
  name: fileName
  type: string
- description: Whether Anypoint Monitoring is enabled for this application
  name: monitoringEnabled
  type: boolean
- description: Whether the platform automatically restarts the application on failure
  name: monitoringAutoRestart
  type: boolean
- description: Whether static IP addresses are allocated to this application
  name: staticIPsEnabled
  type: boolean
- description: Whether persistent queues are enabled for reliable message processing
  name: persistentQueues
  type: boolean
- description: Whether persistent queue data is encrypted at rest
  name: persistentQueuesEncrypted
  type: boolean
- description: Whether the application uses the legacy Object Store v1
  name: objectStoreV1
  type: boolean
- description: Whether the application uses Object Store v2
  name: objectStoreV2
  type: boolean
- description: Whether next-generation logging with Anypoint Monitoring is enabled
  name: loggingNgEnabled
  type: boolean
- description: ''
  name: trackingSettings
  type: object
- description: List of IP addresses assigned to the application workers
  name: ipAddresses
  type: array
- description: ''
  name: vpnConfig
  type: object
- description: Custom log level configuration for application packages
  name: logLevels
  type: array
provider_name: MuleSoft
provider_slug: mulesoft
schema_file: json-schema/mulesoft-application-schema.json
slug: mulesoft-application
source_filename: mulesoft-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://anypoint.mulesoft.com/schemas/mulesoft/application.json\",\n  \"title\": \"MuleSoft Anypoint Application\",\n  \"description\": \"Schema for a Mule application deployed to the Anypoint Platform, including configuration for CloudHub, Runtime Fabric, and hybrid deployment targets.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Unique domain name for the application, used as the subdomain in the CloudHub URL\",\n      \"pattern\": \"^[a-z0-9-]+$\"\n    },\n    \"fullDomain\": {\n      \"type\": \"string\",\n      \"description\": \"Full domain including the platform suffix (e.g., myapp.cloudhub.io)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current deployment status of the application\",\n      \"enum\": [\n        \"\
  STARTED\",\n        \"STARTING\",\n        \"STOPPED\",\n        \"UNDEPLOYED\",\n        \"DEPLOYING\",\n        \"DEPLOY_FAILED\",\n        \"UPDATING\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the application purpose and functionality\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of the organization that owns this application\"\n    },\n    \"environmentId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of the environment where this application is deployed\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud region where the application is deployed\",\n      \"examples\": [\n        \"us-east-1\",\n        \"us-west-2\",\n        \"eu-west-1\",\n        \"eu-central-1\",\n        \"ap-southeast-1\",\n        \"ap-southeast-2\"\
  ,\n        \"ap-northeast-1\",\n        \"ca-central-1\",\n        \"sa-east-1\"\n      ]\n    },\n    \"muleVersion\": {\n      \"$ref\": \"#/$defs/MuleVersion\"\n    },\n    \"workers\": {\n      \"$ref\": \"#/$defs/WorkerConfig\"\n    },\n    \"deploymentTarget\": {\n      \"type\": \"string\",\n      \"description\": \"The target platform for deployment\",\n      \"enum\": [\n        \"cloudhub\",\n        \"cloudhub2\",\n        \"rtf\",\n        \"hybrid\"\n      ]\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Application properties passed as runtime configuration to the Mule runtime\"\n    },\n    \"secureProperties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of property keys that are treated as secure and masked in the UI\"\n    },\n    \"lastUpdateTime\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last application update or redeployment\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the application was first created\"\n    },\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the deployed application archive file (JAR or ZIP)\"\n    },\n    \"monitoringEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Anypoint Monitoring is enabled for this application\",\n      \"default\": true\n    },\n    \"monitoringAutoRestart\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the platform automatically restarts the application on failure\",\n      \"default\": true\n    },\n    \"staticIPsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether static IP addresses are allocated to this application\",\n      \"default\": false\n\
  \    },\n    \"persistentQueues\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether persistent queues are enabled for reliable message processing\",\n      \"default\": false\n    },\n    \"persistentQueuesEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether persistent queue data is encrypted at rest\",\n      \"default\": false\n    },\n    \"objectStoreV1\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application uses the legacy Object Store v1\",\n      \"default\": false\n    },\n    \"objectStoreV2\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application uses Object Store v2\",\n      \"default\": true\n    },\n    \"loggingNgEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether next-generation logging with Anypoint Monitoring is enabled\",\n      \"default\": true\n    },\n    \"trackingSettings\": {\n      \"$ref\": \"#/$defs/TrackingSettings\"\n    },\n    \"\
  ipAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"ipv4\"\n      },\n      \"description\": \"List of IP addresses assigned to the application workers\"\n    },\n    \"vpnConfig\": {\n      \"$ref\": \"#/$defs/VpnConfig\"\n    },\n    \"logLevels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LogLevel\"\n      },\n      \"description\": \"Custom log level configuration for application packages\"\n    }\n  },\n  \"$defs\": {\n    \"MuleVersion\": {\n      \"type\": \"object\",\n      \"description\": \"Mule runtime version information for the deployed application\",\n      \"required\": [\n        \"version\"\n      ],\n      \"properties\": {\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Mule runtime version string (e.g., 4.6.0)\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\\d+(-[a-zA-Z0-9]+)?$\"\n        },\n        \"updateId\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Runtime update identifier for patch-level updates\"\n        },\n        \"endOfSupportDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Date when this runtime version reaches end of support\"\n        }\n      }\n    },\n    \"WorkerConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Worker configuration defining compute resources allocated to the application\",\n      \"required\": [\n        \"amount\",\n        \"type\"\n      ],\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of worker instances running the application\",\n          \"minimum\": 1,\n          \"maximum\": 8\n        },\n        \"type\": {\n          \"type\": \"object\",\n          \"description\": \"Worker type defining the vCore allocation and memory\",\n          \"properties\": {\n            \"\
  name\": {\n              \"type\": \"string\",\n              \"description\": \"Worker size name\",\n              \"enum\": [\n                \"Micro\",\n                \"Small\",\n                \"Medium\",\n                \"Large\",\n                \"xLarge\",\n                \"xxLarge\",\n                \"4xLarge\"\n              ]\n            },\n            \"weight\": {\n              \"type\": \"number\",\n              \"description\": \"vCore weight of the worker type\",\n              \"enum\": [\n                0.1,\n                0.2,\n                1,\n                2,\n                4,\n                8,\n                16\n              ]\n            },\n            \"cpu\": {\n              \"type\": \"string\",\n              \"description\": \"CPU allocation description\"\n            },\n            \"memory\": {\n              \"type\": \"string\",\n              \"description\": \"Memory allocation description (e.g., 500 MB, 1.5 GB)\"\n      \
  \      }\n          }\n        },\n        \"remainingOrgWorkers\": {\n          \"type\": \"number\",\n          \"description\": \"Remaining vCore allocation available in the organization after this application\"\n        }\n      }\n    },\n    \"TrackingSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Transaction tracking configuration for API analytics and debugging\",\n      \"properties\": {\n        \"trackingLevel\": {\n          \"type\": \"string\",\n          \"description\": \"Level of transaction tracking detail\",\n          \"enum\": [\n            \"DISABLED\",\n            \"API_ANALYTICS\",\n            \"DEBUG\"\n          ]\n        }\n      }\n    },\n    \"VpnConfig\": {\n      \"type\": \"object\",\n      \"description\": \"VPN configuration for connecting the application to a private network\",\n      \"properties\": {\n        \"vpnId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the Anypoint VPN connection\"\
  \n        },\n        \"vpcId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the Anypoint Virtual Private Cloud\"\n        },\n        \"vpcName\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the VPC\"\n        }\n      }\n    },\n    \"LogLevel\": {\n      \"type\": \"object\",\n      \"description\": \"Custom log level override for a specific package or class\",\n      \"required\": [\n        \"packageName\",\n        \"level\"\n      ],\n      \"properties\": {\n        \"packageName\": {\n          \"type\": \"string\",\n          \"description\": \"Fully qualified Java package or class name\"\n        },\n        \"level\": {\n          \"type\": \"string\",\n          \"description\": \"Log level to apply\",\n          \"enum\": [\n            \"DEBUG\",\n            \"INFO\",\n            \"WARN\",\n            \"ERROR\",\n            \"OFF\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/json-schema/mulesoft-application-schema.json
tags:
- API Gateway
- API Management
- Enterprise
- Integration
title: MuleSoft Anypoint Application
---
