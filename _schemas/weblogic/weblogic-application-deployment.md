---
description: Configuration schema for an Oracle WebLogic Server application deployment including source path, targets, staging mode, and security model.
layout: schema
name: WebLogic Application Deployment
properties_list:
- description: Application deployment name
  name: name
  type: string
- description: Path to the application archive (EAR, WAR, JAR) or exploded directory on the administration server
  name: sourcePath
  type: string
- description: Target servers or clusters where this application is deployed
  name: targets
  type: array
- description: Type of the application module
  name: moduleType
  type: string
- description: Path to the deployment plan XML file
  name: planPath
  type: string
- description: Root directory for the deployment plan
  name: planDir
  type: string
- description: How the application is staged on target servers
  name: stagingMode
  type: string
- description: How the deployment plan is staged on target servers
  name: planStagingMode
  type: string
- description: Security deployment descriptor model that determines how security roles and policies are managed
  name: securityDDModel
  type: string
- description: Version identifier for the application used in production redeployment
  name: versionIdentifier
  type: string
- description: Order in which this application is deployed relative to other deployments. Lower values are deployed first.
  name: deploymentOrder
  type: integer
- description: Principal name used for deployment authorization
  name: deploymentPrincipalName
  type: string
- description: Optional notes about the deployment
  name: notes
  type: string
- description: Whether modules within an EAR are deployed in parallel
  name: parallelDeployModules
  type: boolean
- description: Whether compiled JSPs and generated classes are cached in the application directory
  name: cacheInAppDirectory
  type: boolean
- description: Whether to validate security data in deployment descriptors
  name: validateDDSecurityData
  type: boolean
provider_name: Oracle WebLogic Server APIs
provider_slug: weblogic
schema_file: json-schema/weblogic-application-deployment.json
slug: weblogic-application-deployment
source_filename: weblogic-application-deployment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/weblogic/application-deployment\",\n  \"title\": \"WebLogic Application Deployment\",\n  \"description\": \"Configuration schema for an Oracle WebLogic Server application deployment including source path, targets, staging mode, and security model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application deployment name\",\n      \"minLength\": 1\n    },\n    \"sourcePath\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the application archive (EAR, WAR, JAR) or exploded directory on the administration server\"\n    },\n    \"targets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Target servers or clusters where this application is deployed\"\n    },\n    \"moduleType\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Type of the application module\",\n      \"enum\": [\"ear\", \"war\", \"jar\", \"rar\"]\n    },\n    \"planPath\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the deployment plan XML file\"\n    },\n    \"planDir\": {\n      \"type\": \"string\",\n      \"description\": \"Root directory for the deployment plan\"\n    },\n    \"stagingMode\": {\n      \"type\": \"string\",\n      \"description\": \"How the application is staged on target servers\",\n      \"enum\": [\"stage\", \"nostage\", \"external_stage\"]\n    },\n    \"planStagingMode\": {\n      \"type\": \"string\",\n      \"description\": \"How the deployment plan is staged on target servers\",\n      \"enum\": [\"stage\", \"nostage\", \"external_stage\"]\n    },\n    \"securityDDModel\": {\n      \"type\": \"string\",\n      \"description\": \"Security deployment descriptor model that determines how security roles and policies are managed\",\n      \"enum\": [\"DDOnly\", \"CustomRoles\"\
  , \"CustomRolesAndPolicies\", \"Advanced\"],\n      \"default\": \"DDOnly\"\n    },\n    \"versionIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Version identifier for the application used in production redeployment\"\n    },\n    \"deploymentOrder\": {\n      \"type\": \"integer\",\n      \"description\": \"Order in which this application is deployed relative to other deployments. Lower values are deployed first.\",\n      \"default\": 100,\n      \"minimum\": 0\n    },\n    \"deploymentPrincipalName\": {\n      \"type\": \"string\",\n      \"description\": \"Principal name used for deployment authorization\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Optional notes about the deployment\"\n    },\n    \"parallelDeployModules\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether modules within an EAR are deployed in parallel\",\n      \"default\": false\n    },\n    \"cacheInAppDirectory\": {\n      \"type\":\
  \ \"boolean\",\n      \"description\": \"Whether compiled JSPs and generated classes are cached in the application directory\",\n      \"default\": false\n    },\n    \"validateDDSecurityData\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to validate security data in deployment descriptors\",\n      \"default\": false\n    }\n  },\n  \"required\": [\"name\", \"sourcePath\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/json-schema/weblogic-application-deployment.json
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
- WebLogic
title: WebLogic Application Deployment
---
