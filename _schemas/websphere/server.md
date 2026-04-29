---
description: Represents an IBM WebSphere Application Server or Liberty server instance, including its configuration, runtime status, resource allocations, and management properties.
layout: schema
name: WebSphere Server
properties_list:
- description: The unique name of the server instance.
  name: name
  type: string
- description: Human-readable display name for the server.
  name: displayName
  type: string
- description: Description of the server purpose.
  name: description
  type: string
- description: Type of server.
  name: serverType
  type: string
- description: Current runtime status of the server.
  name: status
  type: string
- description: Name of the node where this server resides.
  name: nodeName
  type: string
- description: Name of the cell this server belongs to.
  name: cellName
  type: string
- description: Name of the cluster this server is a member of, if any.
  name: clusterName
  type: string
- description: Hostname or IP address of the machine running this server.
  name: hostName
  type: string
- description: WebSphere product version.
  name: version
  type: string
- description: Product edition (e.g., Base, Network Deployment, Liberty).
  name: productEdition
  type: string
- description: Operating system process ID of the running server.
  name: pid
  type: integer
- description: Server uptime in milliseconds.
  name: uptime
  type: integer
- description: Installation directory path.
  name: installDirectory
  type: string
- description: Server-specific configuration directory path.
  name: serverDirectory
  type: string
- description: Network ports configured for this server.
  name: ports
  type: array
- description: JVM configuration for this server.
  name: jvmConfig
  type: object
- description: Enabled Liberty features (Liberty servers only).
  name: features
  type: array
- description: Web container configuration.
  name: webContainer
  type: object
- description: Logging configuration.
  name: logging
  type: object
- description: Applications deployed on this server.
  name: applications
  type: array
- description: Data sources configured on this server.
  name: dataSources
  type: array
- description: Date and time the server was created.
  name: createdDate
  type: string
- description: Date and time the server was last started.
  name: lastStarted
  type: string
- description: Additional metadata associated with the server.
  name: metadata
  type: object
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/server.json
slug: server
source_filename: server.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"server.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebSphere Server\",\n  \"description\": \"Represents an IBM WebSphere Application Server or Liberty server instance, including its configuration, runtime status, resource allocations, and management properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the server instance.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the server.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the server purpose.\"\n    },\n    \"serverType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"APPLICATION_SERVER\",\n        \"WEB_SERVER\",\n        \"PROXY_SERVER\",\n        \"GENERIC_SERVER\",\n        \"LIBERTY\"\n      ],\n      \"description\"\
  : \"Type of server.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"STARTED\", \"STOPPED\", \"STARTING\", \"STOPPING\", \"UNKNOWN\"],\n      \"description\": \"Current runtime status of the server.\"\n    },\n    \"nodeName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the node where this server resides.\"\n    },\n    \"cellName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cell this server belongs to.\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the cluster this server is a member of, if any.\"\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or IP address of the machine running this server.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"WebSphere product version.\",\n      \"examples\": [\"9.0.5.14\", \"24.0.0.3\"]\n    },\n    \"productEdition\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Product edition (e.g., Base, Network Deployment, Liberty).\",\n      \"enum\": [\"BASE\", \"NETWORK_DEPLOYMENT\", \"EXPRESS\", \"LIBERTY_BASE\", \"LIBERTY_CORE\", \"LIBERTY_ND\", \"OPEN_LIBERTY\"]\n    },\n    \"pid\": {\n      \"type\": \"integer\",\n      \"description\": \"Operating system process ID of the running server.\"\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Server uptime in milliseconds.\"\n    },\n    \"installDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Installation directory path.\"\n    },\n    \"serverDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Server-specific configuration directory path.\"\n    },\n    \"ports\": {\n      \"type\": \"array\",\n      \"description\": \"Network ports configured for this server.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n \
  \           \"description\": \"Port name (e.g., WC_defaulthost, WC_defaulthost_secure, BOOTSTRAP_ADDRESS).\"\n          },\n          \"port\": {\n            \"type\": \"integer\",\n            \"minimum\": 1,\n            \"maximum\": 65535,\n            \"description\": \"Port number.\"\n          },\n          \"host\": {\n            \"type\": \"string\",\n            \"description\": \"Host binding for this port.\"\n          },\n          \"protocol\": {\n            \"type\": \"string\",\n            \"enum\": [\"HTTP\", \"HTTPS\", \"IIOP\", \"IIOPS\", \"SIB\", \"SIB_SSL\", \"BOOTSTRAP\", \"SOAP\", \"RMI\"],\n            \"description\": \"Protocol used on this port.\"\n          }\n        },\n        \"required\": [\"name\", \"port\"]\n      }\n    },\n    \"jvmConfig\": {\n      \"type\": \"object\",\n      \"description\": \"JVM configuration for this server.\",\n      \"properties\": {\n        \"javaVersion\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Java runtime version.\"\n        },\n        \"javaVendor\": {\n          \"type\": \"string\",\n          \"description\": \"Java vendor (e.g., IBM, Eclipse Adoptium).\"\n        },\n        \"javaHome\": {\n          \"type\": \"string\",\n          \"description\": \"Java home directory.\"\n        },\n        \"initialHeapSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Initial JVM heap size in MB.\"\n        },\n        \"maximumHeapSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum JVM heap size in MB.\"\n        },\n        \"genericJvmArguments\": {\n          \"type\": \"string\",\n          \"description\": \"Additional JVM arguments.\"\n        }\n      }\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"Enabled Liberty features (Liberty servers only).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [[\"webProfile-10.0\", \"restConnector-2.0\", \"\
  mpHealth-4.0\"]]\n    },\n    \"webContainer\": {\n      \"type\": \"object\",\n      \"description\": \"Web container configuration.\",\n      \"properties\": {\n        \"threadPool\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"minimumSize\": {\n              \"type\": \"integer\"\n            },\n            \"maximumSize\": {\n              \"type\": \"integer\"\n            }\n          }\n        },\n        \"sessionTimeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Default session timeout in minutes.\"\n        }\n      }\n    },\n    \"logging\": {\n      \"type\": \"object\",\n      \"description\": \"Logging configuration.\",\n      \"properties\": {\n        \"logDirectory\": {\n          \"type\": \"string\",\n          \"description\": \"Log output directory.\"\n        },\n        \"consoleLogLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\"AUDIT\", \"INFO\", \"WARNING\", \"ERROR\", \"OFF\"\
  ]\n        },\n        \"traceSpecification\": {\n          \"type\": \"string\",\n          \"description\": \"Trace specification string.\"\n        },\n        \"maxFileSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum log file size in MB.\"\n        },\n        \"maxFiles\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of log files to retain.\"\n        }\n      }\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"description\": \"Applications deployed on this server.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"dataSources\": {\n      \"type\": \"array\",\n      \"description\": \"Data sources configured on this server.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"jndiName\": {\n            \"type\": \"string\"\n          },\n          \"databaseType\"\
  : {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the server was created.\"\n    },\n    \"lastStarted\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the server was last started.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Additional metadata associated with the server.\"\n    }\n  },\n  \"required\": [\"name\", \"serverType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/server.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: WebSphere Server
---
