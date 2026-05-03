---
description: Configuration schema for an Oracle WebLogic Server instance including listen ports, cluster membership, staging mode, and SSL settings.
layout: schema
name: WebLogic Server Configuration
properties_list:
- description: Unique name of the server instance within the domain
  name: name
  type: string
- description: Network address on which the server listens for connections. Empty string means all available addresses.
  name: listenAddress
  type: string
- description: Non-SSL listen port for the server
  name: listenPort
  type: integer
- description: Whether the plain-text (non-SSL) listen port is enabled
  name: listenPortEnabled
  type: boolean
- description: SSL listen port for the server
  name: SSLListenPort
  type: integer
- description: Whether SSL is enabled for this server
  name: SSLEnabled
  type: boolean
- description: Name of the cluster this server belongs to, or null if standalone
  name: cluster
  type:
  - string
  - 'null'
- description: Name of the machine (Node Manager) this server is assigned to
  name: machine
  type:
  - string
  - 'null'
- description: The initial running state when the server starts
  name: startupMode
  type: string
- description: Whether the Node Manager should automatically restart this server if it fails
  name: autoRestart
  type: boolean
- description: Maximum number of times Node Manager will attempt to restart this server
  name: restartMax
  type: integer
- description: Interval in seconds within which restartMax restarts must occur to trigger failure
  name: restartIntervalSeconds
  type: integer
- description: How applications are staged on this server
  name: stagingMode
  type: string
- description: Directory used for staging deployed applications
  name: stagingDirectoryName
  type: string
- description: Directory used for uploaded deployment files
  name: uploadDirectoryName
  type: string
- description: Java compiler to use for JSP compilation
  name: javaCompiler
  type: string
- description: Whether the server should accept client certificate proxy headers from a web server plugin
  name: clientCertProxyEnabled
  type: boolean
- description: Whether to use the WebLogic Plugin for proxy requests
  name: weblogicPluginEnabled
  type: boolean
- description: Timeout in seconds for graceful shutdown
  name: gracefulShutdownTimeout
  type: integer
- description: Server log configuration
  name: log
  type: object
- description: SSL/TLS configuration for the server
  name: SSL
  type: object
- description: Custom network channels configured on this server
  name: networkAccessPoints
  type: array
provider_name: Oracle WebLogic Server APIs
provider_slug: weblogic
schema_file: json-schema/weblogic-server-configuration.json
slug: weblogic-server-configuration
source_filename: weblogic-server-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/weblogic/server-configuration\",\n  \"title\": \"WebLogic Server Configuration\",\n  \"description\": \"Configuration schema for an Oracle WebLogic Server instance including listen ports, cluster membership, staging mode, and SSL settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the server instance within the domain\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"listenAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Network address on which the server listens for connections. Empty string means all available addresses.\",\n      \"default\": \"\"\n    },\n    \"listenPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Non-SSL listen port for the server\",\n      \"default\": 7001,\n      \"minimum\": 1,\n      \"maximum\"\
  : 65535\n    },\n    \"listenPortEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the plain-text (non-SSL) listen port is enabled\",\n      \"default\": true\n    },\n    \"SSLListenPort\": {\n      \"type\": \"integer\",\n      \"description\": \"SSL listen port for the server\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"SSLEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SSL is enabled for this server\",\n      \"default\": false\n    },\n    \"cluster\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of the cluster this server belongs to, or null if standalone\"\n    },\n    \"machine\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of the machine (Node Manager) this server is assigned to\"\n    },\n    \"startupMode\": {\n      \"type\": \"string\",\n      \"description\": \"The initial running state when the server starts\",\n      \"enum\": [\"RUNNING\"\
  , \"STANDBY\", \"ADMIN\"],\n      \"default\": \"RUNNING\"\n    },\n    \"autoRestart\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Node Manager should automatically restart this server if it fails\",\n      \"default\": true\n    },\n    \"restartMax\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of times Node Manager will attempt to restart this server\",\n      \"default\": 2,\n      \"minimum\": 0\n    },\n    \"restartIntervalSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Interval in seconds within which restartMax restarts must occur to trigger failure\",\n      \"default\": 3600,\n      \"minimum\": 0\n    },\n    \"stagingMode\": {\n      \"type\": \"string\",\n      \"description\": \"How applications are staged on this server\",\n      \"enum\": [\"stage\", \"nostage\", \"external_stage\"],\n      \"default\": \"stage\"\n    },\n    \"stagingDirectoryName\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Directory used for staging deployed applications\"\n    },\n    \"uploadDirectoryName\": {\n      \"type\": \"string\",\n      \"description\": \"Directory used for uploaded deployment files\"\n    },\n    \"javaCompiler\": {\n      \"type\": \"string\",\n      \"description\": \"Java compiler to use for JSP compilation\"\n    },\n    \"clientCertProxyEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the server should accept client certificate proxy headers from a web server plugin\",\n      \"default\": false\n    },\n    \"weblogicPluginEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use the WebLogic Plugin for proxy requests\",\n      \"default\": false\n    },\n    \"gracefulShutdownTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds for graceful shutdown\",\n      \"default\": 0,\n      \"minimum\": 0\n    },\n    \"log\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Server log configuration\",\n      \"properties\": {\n        \"fileName\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the server log file\"\n        },\n        \"fileMinSize\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum size in kilobytes before the log file is rotated\",\n          \"default\": 5000\n        },\n        \"rotationType\": {\n          \"type\": \"string\",\n          \"description\": \"Log rotation strategy\",\n          \"enum\": [\"bySize\", \"byTime\", \"none\"],\n          \"default\": \"bySize\"\n        },\n        \"numberOfFilesLimited\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the number of rotated log files is limited\",\n          \"default\": true\n        },\n        \"fileCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of rotated log files to keep\",\n          \"default\": 7\n        },\n        \"rotateLogOnStartup\"\
  : {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to rotate the log file when the server starts\",\n          \"default\": true\n        },\n        \"logFileSeverity\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum severity of messages written to the log file\",\n          \"enum\": [\"Debug\", \"Info\", \"Notice\", \"Warning\", \"Error\", \"Critical\", \"Alert\", \"Emergency\", \"Off\"],\n          \"default\": \"Debug\"\n        },\n        \"stdoutSeverity\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum severity of messages written to standard out\",\n          \"enum\": [\"Debug\", \"Info\", \"Notice\", \"Warning\", \"Error\", \"Critical\", \"Alert\", \"Emergency\", \"Off\"],\n          \"default\": \"Notice\"\n        }\n      }\n    },\n    \"SSL\": {\n      \"type\": \"object\",\n      \"description\": \"SSL/TLS configuration for the server\",\n      \"properties\": {\n        \"enabled\": {\n    \
  \      \"type\": \"boolean\",\n          \"default\": false\n        },\n        \"listenPort\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 65535\n        },\n        \"twoWaySSLEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether two-way (mutual) SSL is enabled\",\n          \"default\": false\n        },\n        \"clientCertificateEnforced\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether client certificates are enforced\",\n          \"default\": false\n        },\n        \"jSSEEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether JSSE SSL implementation is used\",\n          \"default\": true\n        },\n        \"minimumTLSProtocolVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum TLS protocol version allowed\",\n          \"enum\": [\"TLSv1\", \"TLSv1.1\", \"TLSv1.2\", \"TLSv1.3\"]\n        }\n      }\n    },\n \
  \   \"networkAccessPoints\": {\n      \"type\": \"array\",\n      \"description\": \"Custom network channels configured on this server\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Channel name\"\n          },\n          \"protocol\": {\n            \"type\": \"string\",\n            \"description\": \"Protocol for the channel\",\n            \"enum\": [\"t3\", \"t3s\", \"http\", \"https\", \"iiop\", \"iiops\", \"admin\"]\n          },\n          \"listenAddress\": {\n            \"type\": \"string\"\n          },\n          \"listenPort\": {\n            \"type\": \"integer\",\n            \"minimum\": 1,\n            \"maximum\": 65535\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"default\": true\n          }\n        },\n        \"required\": [\"name\", \"protocol\", \"listenPort\"]\n      }\n    }\n  },\n  \"required\"\
  : [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/json-schema/weblogic-server-configuration.json
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
- WebLogic
title: WebLogic Server Configuration
---
