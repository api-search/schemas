---
description: Schema for WebLogic Server instance configuration as exposed through the RESTful Management API edit tree.
layout: schema
name: Oracle WebLogic Server Configuration
properties_list:
- description: Bean identity path as an array of path segments (e.g., ['domain', 'servers', 'Server-0'])
  name: identity
  type: array
- description: Unique name identifying this server within the domain
  name: name
  type: string
- description: Non-SSL listen port for the server
  name: listenPort
  type: integer
- description: IP address or DNS hostname the server listens on. Empty string means all network interfaces.
  name: listenAddress
  type: string
- description: Whether the non-SSL listen port is enabled
  name: listenPortEnabled
  type: boolean
- description: SSL listen port for the server
  name: SSLListenPort
  type: integer
- description: Domain-wide administration port (SSL-only)
  name: administrationPort
  type: integer
- description: Default network protocol for server communication
  name: defaultProtocol
  type: string
- description: Reference to the machine this server runs on
  name: machine
  type: object
- description: Reference to the cluster this server belongs to
  name: cluster
  type: object
- description: Candidate machines for server migration
  name: candidateMachines
  type: array
- description: Idle connection timeout in seconds
  name: idleConnectionTimeout
  type: integer
- description: Replication group name for session state replication
  name: replicationGroup
  type:
  - string
  - 'null'
- description: SSL/TLS configuration for this server
  name: SSL
  type: object
- description: Startup configuration including JVM arguments
  name: serverStart
  type: object
- description: Network channels configured for this server
  name: networkAccessPoints
  type: array
- description: ''
  name: links
  type: array
provider_name: Oracle WebLogic Server
provider_slug: oracle-weblogic
schema_file: json-schema/oracle-weblogic-server-configuration.json
slug: oracle-weblogic-server-configuration
source_filename: oracle-weblogic-server-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/weblogic/server-configuration\",\n  \"title\": \"Oracle WebLogic Server Configuration\",\n  \"description\": \"Schema for WebLogic Server instance configuration as exposed through the RESTful Management API edit tree.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"identity\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Bean identity path as an array of path segments (e.g., ['domain', 'servers', 'Server-0'])\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name identifying this server within the domain\"\n    },\n    \"listenPort\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"default\": 7001,\n      \"description\": \"Non-SSL listen port for the server\"\n    },\n    \"listenAddress\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"IP address or DNS hostname the server listens on. Empty string means all network interfaces.\"\n    },\n    \"listenPortEnabled\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether the non-SSL listen port is enabled\"\n    },\n    \"SSLListenPort\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"description\": \"SSL listen port for the server\"\n    },\n    \"administrationPort\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"description\": \"Domain-wide administration port (SSL-only)\"\n    },\n    \"defaultProtocol\": {\n      \"type\": \"string\",\n      \"enum\": [\"t3\", \"t3s\", \"http\", \"https\", \"iiop\", \"iiops\"],\n      \"description\": \"Default network protocol for server communication\"\n    },\n    \"machine\": {\n      \"$ref\": \"#/$defs/beanReference\",\n      \"description\": \"Reference\
  \ to the machine this server runs on\"\n    },\n    \"cluster\": {\n      \"$ref\": \"#/$defs/beanReference\",\n      \"description\": \"Reference to the cluster this server belongs to\"\n    },\n    \"candidateMachines\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/identityObject\" },\n      \"description\": \"Candidate machines for server migration\"\n    },\n    \"idleConnectionTimeout\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Idle connection timeout in seconds\"\n    },\n    \"replicationGroup\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Replication group name for session state replication\"\n    },\n    \"SSL\": {\n      \"$ref\": \"#/$defs/SSLConfiguration\",\n      \"description\": \"SSL/TLS configuration for this server\"\n    },\n    \"serverStart\": {\n      \"$ref\": \"#/$defs/serverStart\",\n      \"description\": \"Startup configuration including JVM arguments\"\n    },\n    \"networkAccessPoints\"\
  : {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/networkAccessPoint\" },\n      \"description\": \"Network channels configured for this server\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/link\" }\n    }\n  },\n  \"$defs\": {\n    \"beanReference\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Bean reference as an identity path array (e.g., ['machines', 'Machine-0'])\"\n    },\n    \"identityObject\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"identity\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        }\n      },\n      \"required\": [\"identity\"]\n    },\n    \"link\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Link relation type (self, canonical, parent, action, etc.)\"\n        },\n        \"href\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the linked resource\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable title\"\n        }\n      },\n      \"required\": [\"rel\", \"href\"]\n    },\n    \"SSLConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"SSL/TLS configuration for a WebLogic Server\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether SSL is enabled\"\n        },\n        \"listenPort\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 65535,\n          \"description\": \"SSL listen port\"\n        },\n        \"identityAndTrustLocations\": {\n          \"type\": \"string\",\n          \"description\": \"Location of identity and trust keystores\"\n        },\n        \"serverPrivateKeyAlias\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Alias for the server private key in the keystore\"\n        },\n        \"serverPrivateKeyPassPhrase\": {\n          \"type\": \"string\",\n          \"description\": \"Passphrase for the server private key (encrypted)\"\n        },\n        \"twoWaySSLEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether mutual (two-way) SSL is enabled\"\n        },\n        \"clientCertificateEnforced\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether client certificates are required\"\n        },\n        \"hostnameVerificationIgnored\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether hostname verification is skipped\"\n        }\n      }\n    },\n    \"serverStart\": {\n      \"type\": \"object\",\n      \"description\": \"Server startup configuration\",\n      \"properties\": {\n        \"arguments\": {\n          \"type\": \"string\",\n          \"\
  description\": \"JVM arguments for server startup (e.g., -Xmx512m)\"\n        },\n        \"classPath\": {\n          \"type\": \"string\",\n          \"description\": \"Additional classpath entries\"\n        },\n        \"javaHome\": {\n          \"type\": \"string\",\n          \"description\": \"Java home directory path\"\n        },\n        \"javaVendor\": {\n          \"type\": \"string\",\n          \"description\": \"Java vendor name\"\n        },\n        \"beaHome\": {\n          \"type\": \"string\",\n          \"description\": \"Oracle/BEA home directory path\"\n        }\n      }\n    },\n    \"networkAccessPoint\": {\n      \"type\": \"object\",\n      \"description\": \"Network channel configuration for a server\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Network channel name\"\n        },\n        \"protocol\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Network protocol (t3, t3s, http, https, iiop, iiops)\"\n        },\n        \"listenPort\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 65535\n        },\n        \"listenAddress\": { \"type\": \"string\" },\n        \"publicPort\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 65535,\n          \"description\": \"External-facing port (for NAT/load balancer)\"\n        },\n        \"publicAddress\": {\n          \"type\": \"string\",\n          \"description\": \"External-facing address\"\n        },\n        \"enabled\": { \"type\": \"boolean\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-weblogic/refs/heads/main/json-schema/oracle-weblogic-server-configuration.json
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
title: Oracle WebLogic Server Configuration
---
