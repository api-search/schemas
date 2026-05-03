---
description: Schema for WebLogic Server application and library deployment configurations as exposed through the RESTful Management API.
layout: schema
name: Oracle WebLogic Deployment Configuration
properties_list:
- description: Bean identity path
  name: identity
  type: array
- description: Application deployment name
  name: name
  type: string
- description: Filesystem path to the application source (EAR, WAR, or exploded directory)
  name: sourcePath
  type: string
- description: URL or file path for deploying the application (used during creation)
  name: sourceURL
  type: string
- description: Deployment targets (servers and/or clusters)
  name: targets
  type: array
- description: Order in which applications are deployed during domain startup. Lower values deploy first.
  name: deploymentOrder
  type: integer
- description: Path to the deployment plan XML file for customizing deployment descriptors
  name: planPath
  type:
  - string
  - 'null'
- description: Security deployment descriptor model that determines how security roles and policies are sourced
  name: securityDDModel
  type: string
- description: 'How application files are distributed to managed servers: stage copies files, nostage uses the source directly, external_stage uses a pre-staged location'
  name: stagingMode
  type: string
- description: Sub-deployments for module-level targeting
  name: subDeployments
  type: array
- description: ''
  name: links
  type: array
provider_name: Oracle WebLogic Server
provider_slug: oracle-weblogic
schema_file: json-schema/oracle-weblogic-deployment.json
slug: oracle-weblogic-deployment
source_filename: oracle-weblogic-deployment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/weblogic/deployment\",\n  \"title\": \"Oracle WebLogic Deployment Configuration\",\n  \"description\": \"Schema for WebLogic Server application and library deployment configurations as exposed through the RESTful Management API.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"identity\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Bean identity path\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application deployment name\"\n    },\n    \"sourcePath\": {\n      \"type\": \"string\",\n      \"description\": \"Filesystem path to the application source (EAR, WAR, or exploded directory)\"\n    },\n    \"sourceURL\": {\n      \"type\": \"string\",\n      \"description\": \"URL or file path for deploying the application (used during creation)\"\n\
  \    },\n    \"targets\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/identityObject\" },\n      \"description\": \"Deployment targets (servers and/or clusters)\"\n    },\n    \"deploymentOrder\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Order in which applications are deployed during domain startup. Lower values deploy first.\"\n    },\n    \"planPath\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Path to the deployment plan XML file for customizing deployment descriptors\"\n    },\n    \"securityDDModel\": {\n      \"type\": \"string\",\n      \"enum\": [\"DDOnly\", \"CustomRoles\", \"CustomRolesAndPolicies\", \"Advanced\"],\n      \"description\": \"Security deployment descriptor model that determines how security roles and policies are sourced\"\n    },\n    \"stagingMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"stage\", \"nostage\", \"external_stage\"],\n      \"description\": \"\
  How application files are distributed to managed servers: stage copies files, nostage uses the source directly, external_stage uses a pre-staged location\"\n    },\n    \"subDeployments\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/subDeployment\" },\n      \"description\": \"Sub-deployments for module-level targeting\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/link\" }\n    }\n  },\n  \"$defs\": {\n    \"identityObject\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"identity\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Identity path (e.g., ['servers', 'Server-0'] or ['clusters', 'Cluster1'])\"\n        }\n      },\n      \"required\": [\"identity\"]\n    },\n    \"link\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"rel\": { \"type\": \"string\" },\n        \"href\": { \"type\": \"string\", \"format\"\
  : \"uri\" },\n        \"title\": { \"type\": \"string\" }\n      },\n      \"required\": [\"rel\", \"href\"]\n    },\n    \"subDeployment\": {\n      \"type\": \"object\",\n      \"description\": \"Sub-deployment targeting configuration for individual modules within an application\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Sub-deployment name (typically matches the module name)\"\n        },\n        \"targets\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/identityObject\" },\n          \"description\": \"Targets for this sub-deployment\"\n        }\n      }\n    },\n    \"libraryDeployment\": {\n      \"type\": \"object\",\n      \"description\": \"Shared library deployment configuration\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"identity\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n\
  \        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Library deployment name\"\n        },\n        \"sourcePath\": {\n          \"type\": \"string\",\n          \"description\": \"Filesystem path to the library archive\"\n        },\n        \"sourceURL\": {\n          \"type\": \"string\",\n          \"description\": \"URL or file path for deploying the library\"\n        },\n        \"targets\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/identityObject\" }\n        },\n        \"deploymentOrder\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"links\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/link\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/json-schema/oracle-weblogic-deployment.json
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
title: Oracle WebLogic Deployment Configuration
---
