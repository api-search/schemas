---
description: Configuration schema for an Oracle WebLogic Server domain including servers, clusters, data sources, JMS resources, and security configuration.
layout: schema
name: WebLogic Domain Configuration
properties_list:
- description: Domain name
  name: name
  type: string
- description: Name of the administration server for this domain
  name: adminServerName
  type: string
- description: WebLogic Server version of the domain
  name: domainVersion
  type: string
- description: Whether the domain is running in production mode
  name: productionModeEnabled
  type: boolean
- description: Configuration version string
  name: configurationVersion
  type: string
- description: Protocol used for administration communication
  name: administrationProtocol
  type: string
- description: Administration port used when production mode is enabled
  name: administrationPort
  type: integer
- description: Whether the domain-wide administration port is enabled
  name: administrationPortEnabled
  type: boolean
- description: Whether Exalogic-specific optimizations are enabled
  name: exalogicOptimizationsEnabled
  type: boolean
- description: Whether automatic configuration backup is enabled
  name: configBackupEnabled
  type: boolean
- description: Number of configuration archive files to maintain
  name: archiveConfigurationCount
  type: integer
- description: Server instances in the domain
  name: servers
  type: array
- description: Clusters in the domain
  name: clusters
  type: array
- description: JDBC system resources (data sources) in the domain
  name: JDBCSystemResources
  type: array
- description: JMS system resources in the domain
  name: JMSSystemResources
  type: array
- description: Application deployments in the domain
  name: appDeployments
  type: array
- description: Domain security configuration
  name: securityConfiguration
  type: object
provider_name: Oracle WebLogic Server APIs
provider_slug: weblogic
schema_file: json-schema/weblogic-domain-configuration.json
slug: weblogic-domain-configuration
source_filename: weblogic-domain-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/weblogic/domain-configuration\",\n  \"title\": \"WebLogic Domain Configuration\",\n  \"description\": \"Configuration schema for an Oracle WebLogic Server domain including servers, clusters, data sources, JMS resources, and security configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Domain name\",\n      \"minLength\": 1\n    },\n    \"adminServerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the administration server for this domain\"\n    },\n    \"domainVersion\": {\n      \"type\": \"string\",\n      \"description\": \"WebLogic Server version of the domain\"\n    },\n    \"productionModeEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is running in production mode\",\n      \"default\": false\n    },\n    \"configurationVersion\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Configuration version string\"\n    },\n    \"administrationProtocol\": {\n      \"type\": \"string\",\n      \"description\": \"Protocol used for administration communication\",\n      \"enum\": [\"t3s\", \"https\", \"iiops\"],\n      \"default\": \"t3s\"\n    },\n    \"administrationPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Administration port used when production mode is enabled\",\n      \"default\": 9002,\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"administrationPortEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain-wide administration port is enabled\",\n      \"default\": false\n    },\n    \"exalogicOptimizationsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Exalogic-specific optimizations are enabled\",\n      \"default\": false\n    },\n    \"configBackupEnabled\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether automatic configuration backup is enabled\",\n      \"default\": false\n    },\n    \"archiveConfigurationCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of configuration archive files to maintain\",\n      \"default\": 0,\n      \"minimum\": 0\n    },\n    \"servers\": {\n      \"type\": \"array\",\n      \"description\": \"Server instances in the domain\",\n      \"items\": {\n        \"$ref\": \"weblogic-server-configuration.json\"\n      }\n    },\n    \"clusters\": {\n      \"type\": \"array\",\n      \"description\": \"Clusters in the domain\",\n      \"items\": {\n        \"$ref\": \"weblogic-cluster-configuration.json\"\n      }\n    },\n    \"JDBCSystemResources\": {\n      \"type\": \"array\",\n      \"description\": \"JDBC system resources (data sources) in the domain\",\n      \"items\": {\n        \"$ref\": \"weblogic-datasource-configuration.json\"\n      }\n    },\n    \"JMSSystemResources\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"JMS system resources in the domain\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"JMS system resource name\"\n          },\n          \"targets\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Target servers or clusters\"\n          },\n          \"descriptorFileName\": {\n            \"type\": \"string\",\n            \"description\": \"JMS descriptor file name\"\n          }\n        },\n        \"required\": [\"name\"]\n      }\n    },\n    \"appDeployments\": {\n      \"type\": \"array\",\n      \"description\": \"Application deployments in the domain\",\n      \"items\": {\n        \"$ref\": \"weblogic-application-deployment.json\"\n      }\n    },\n    \"securityConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Domain security configuration\"\
  ,\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"realms\": {\n          \"type\": \"array\",\n          \"description\": \"Security realms\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"authenticationProviders\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": {\n                      \"type\": \"string\"\n                    },\n                    \"type\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"crossDomainSecurityEnabled\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"webAppFilesCaseInsensitive\"\
  : {\n          \"type\": \"string\",\n          \"enum\": [\"os\", \"true\", \"false\"],\n          \"default\": \"os\"\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"adminServerName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/json-schema/weblogic-domain-configuration.json
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
- WebLogic
title: WebLogic Domain Configuration
---
