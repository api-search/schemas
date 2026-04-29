---
description: Represents a deployed application in IBM WebSphere Application Server or Liberty, including its configuration, modules, deployment targets, and runtime status.
layout: schema
name: WebSphere Application
properties_list:
- description: The unique name of the application within the server or cell.
  name: name
  type: string
- description: Human-readable display name for the application.
  name: displayName
  type: string
- description: Description of the application purpose and functionality.
  name: description
  type: string
- description: Current runtime status of the application.
  name: status
  type: string
- description: Application archive type.
  name: type
  type: string
- description: Context root for web modules within the application.
  name: contextRoot
  type: string
- description: File system location of the application archive or directory.
  name: location
  type: string
- description: Whether the application starts automatically when the server starts.
  name: autoStart
  type: boolean
- description: Name of the server where the application is deployed.
  name: targetServer
  type: string
- description: Name of the cluster where the application is deployed.
  name: targetCluster
  type: string
- description: Application modules contained within the deployment.
  name: modules
  type: array
- description: Class loader policy for the application.
  name: classloaderPolicy
  type: string
- description: Class loading delegation mode.
  name: classloaderMode
  type: string
- description: Security roles defined in the application.
  name: securityRoles
  type: array
- description: Session management configuration.
  name: sessionManagement
  type: object
- description: Application version identifier.
  name: version
  type: string
- description: Date and time the application was deployed.
  name: deployedDate
  type: string
- description: Date and time the application was last modified.
  name: lastModified
  type: string
- description: Additional metadata associated with the application.
  name: metadata
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/application.json
slug: application
source_filename: application.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"application.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebSphere Application\",\n  \"description\": \"Represents a deployed application in IBM WebSphere Application Server or Liberty, including its configuration, modules, deployment targets, and runtime status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the application within the server or cell.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the application.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the application purpose and functionality.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"started\", \"stopped\", \"starting\", \"stopping\", \"installed\", \"unknown\"],\n      \"description\": \"Current runtime\
  \ status of the application.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"ear\", \"war\", \"jar\", \"eba\", \"rar\"],\n      \"description\": \"Application archive type.\"\n    },\n    \"contextRoot\": {\n      \"type\": \"string\",\n      \"description\": \"Context root for web modules within the application.\",\n      \"examples\": [\"/myapp\"]\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"File system location of the application archive or directory.\"\n    },\n    \"autoStart\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether the application starts automatically when the server starts.\"\n    },\n    \"targetServer\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the server where the application is deployed.\"\n    },\n    \"targetCluster\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cluster where the application is deployed.\"\
  \n    },\n    \"modules\": {\n      \"type\": \"array\",\n      \"description\": \"Application modules contained within the deployment.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Module name.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"web\", \"ejb\", \"connector\", \"client\", \"utility\"],\n            \"description\": \"Module type.\"\n          },\n          \"uri\": {\n            \"type\": \"string\",\n            \"description\": \"URI of the module within the application archive.\"\n          },\n          \"contextRoot\": {\n            \"type\": \"string\",\n            \"description\": \"Context root for web modules.\"\n          },\n          \"targetServer\": {\n            \"type\": \"string\",\n            \"description\": \"Target server for this module.\"\n          }\n        },\n      \
  \  \"required\": [\"name\", \"type\"]\n      }\n    },\n    \"classloaderPolicy\": {\n      \"type\": \"string\",\n      \"enum\": [\"SINGLE\", \"MULTIPLE\"],\n      \"description\": \"Class loader policy for the application.\"\n    },\n    \"classloaderMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"PARENT_FIRST\", \"PARENT_LAST\"],\n      \"description\": \"Class loading delegation mode.\"\n    },\n    \"securityRoles\": {\n      \"type\": \"array\",\n      \"description\": \"Security roles defined in the application.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Security role name.\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"mappedUsers\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Users\
  \ mapped to this role.\"\n          },\n          \"mappedGroups\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Groups mapped to this role.\"\n          }\n        },\n        \"required\": [\"name\"]\n      }\n    },\n    \"sessionManagement\": {\n      \"type\": \"object\",\n      \"description\": \"Session management configuration.\",\n      \"properties\": {\n        \"sessionTimeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Session timeout in minutes.\"\n        },\n        \"enableCookies\": {\n          \"type\": \"boolean\",\n          \"default\": true\n        },\n        \"enableURLRewriting\": {\n          \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"persistenceMode\": {\n          \"type\": \"string\",\n          \"enum\": [\"NONE\", \"DATABASE\", \"MEMORY_TO_MEMORY\", \"DATA_REPLICATION\"],\n          \"description\"\
  : \"Session persistence mode.\"\n        }\n      }\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Application version identifier.\"\n    },\n    \"deployedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the application was deployed.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the application was last modified.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Additional metadata associated with the application.\"\n    }\n  },\n  \"required\": [\"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/application.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: WebSphere Application
---
