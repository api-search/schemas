---
description: Runtime data schema for an Oracle WebLogic Server instance including state, health, JVM metrics, thread pool statistics, and subsystem runtimes.
layout: schema
name: WebLogic Server Runtime
properties_list:
- description: Server instance name
  name: name
  type: string
- description: Current server lifecycle state
  name: state
  type: string
- description: Current listen address
  name: listenAddress
  type: string
- description: Current listen port
  name: listenPort
  type: integer
- description: Current SSL listen port
  name: SSLListenPort
  type: integer
- description: Administration server hostname
  name: adminServerHost
  type: string
- description: Administration server listen port
  name: adminServerListenPort
  type: integer
- description: Machine the server is currently running on
  name: currentMachine
  type: string
- description: WebLogic Server version string
  name: weblogicVersion
  type: string
- description: Server activation time in milliseconds since epoch
  name: activationTime
  type: integer
- description: Current number of open sockets
  name: openSocketsCurrentCount
  type: integer
- description: Whether a server restart is required to apply pending changes
  name: restartRequired
  type: boolean
- description: ''
  name: healthState
  type: object
- description: ''
  name: overallHealthState
  type: object
- description: JVM runtime metrics
  name: JVMRuntime
  type: object
- description: Thread pool runtime metrics
  name: threadPoolRuntime
  type: object
- description: JDBC service runtime
  name: JDBCServiceRuntime
  type: object
- description: JMS runtime
  name: JMSRuntime
  type: object
- description: Runtime information for deployed applications
  name: applicationRuntimes
  type: array
provider_name: Oracle WebLogic Server APIs
provider_slug: weblogic
schema_file: json-schema/weblogic-server-runtime.json
slug: weblogic-server-runtime
source_filename: weblogic-server-runtime.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/weblogic/server-runtime\",\n  \"title\": \"WebLogic Server Runtime\",\n  \"description\": \"Runtime data schema for an Oracle WebLogic Server instance including state, health, JVM metrics, thread pool statistics, and subsystem runtimes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Server instance name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current server lifecycle state\",\n      \"enum\": [\n        \"SHUTDOWN\",\n        \"STARTING\",\n        \"STANDBY\",\n        \"ADMIN\",\n        \"RESUMING\",\n        \"RUNNING\",\n        \"SUSPENDING\",\n        \"FORCE_SUSPENDING\",\n        \"SHUTTING_DOWN\",\n        \"FAILED\",\n        \"UNKNOWN\"\n      ]\n    },\n    \"listenAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Current\
  \ listen address\"\n    },\n    \"listenPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Current listen port\"\n    },\n    \"SSLListenPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Current SSL listen port\"\n    },\n    \"adminServerHost\": {\n      \"type\": \"string\",\n      \"description\": \"Administration server hostname\"\n    },\n    \"adminServerListenPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Administration server listen port\"\n    },\n    \"currentMachine\": {\n      \"type\": \"string\",\n      \"description\": \"Machine the server is currently running on\"\n    },\n    \"weblogicVersion\": {\n      \"type\": \"string\",\n      \"description\": \"WebLogic Server version string\"\n    },\n    \"activationTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Server activation time in milliseconds since epoch\"\n    },\n    \"openSocketsCurrentCount\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Current number of open sockets\"\n    },\n    \"restartRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a server restart is required to apply pending changes\"\n    },\n    \"healthState\": {\n      \"$ref\": \"#/$defs/HealthState\"\n    },\n    \"overallHealthState\": {\n      \"$ref\": \"#/$defs/HealthState\"\n    },\n    \"JVMRuntime\": {\n      \"type\": \"object\",\n      \"description\": \"JVM runtime metrics\",\n      \"properties\": {\n        \"heapSizeCurrent\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Current JVM heap size in bytes\"\n        },\n        \"heapSizeMax\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum JVM heap size in bytes\"\n        },\n        \"heapFreeCurrent\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Current free heap memory\
  \ in bytes\"\n        },\n        \"heapFreePercent\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Percentage of heap memory that is free\"\n        },\n        \"javaVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Java version\"\n        },\n        \"javaVendor\": {\n          \"type\": \"string\",\n          \"description\": \"Java vendor\"\n        },\n        \"osName\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system name\"\n        },\n        \"osVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system version\"\n        },\n        \"uptime\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"JVM uptime in milliseconds\"\n        }\n      }\n    },\n    \"threadPoolRuntime\": {\n      \"type\": \"object\",\n      \"description\": \"Thread pool runtime metrics\",\n      \"properties\"\
  : {\n        \"executeThreadTotalCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of execute threads in the pool\"\n        },\n        \"executeThreadIdleCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of idle execute threads\"\n        },\n        \"hoggingThreadCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of threads hogging resources beyond the configured threshold\"\n        },\n        \"stuckThreadCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of threads stuck beyond the configured stuck thread time\"\n        },\n        \"pendingUserRequestCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of pending user requests in the queue\"\n        },\n        \"throughput\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Thread pool throughput in requests per second\"\
  \n        },\n        \"completedRequestCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Total number of completed requests\"\n        },\n        \"overloadRejectedRequestsCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Number of requests rejected due to server overload\"\n        },\n        \"queueLength\": {\n          \"type\": \"integer\",\n          \"description\": \"Current length of the request queue\"\n        }\n      }\n    },\n    \"JDBCServiceRuntime\": {\n      \"type\": \"object\",\n      \"description\": \"JDBC service runtime\",\n      \"properties\": {\n        \"JDBCDataSourceRuntimeMBeans\": {\n          \"type\": \"array\",\n          \"description\": \"JDBC data source runtime instances\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n\
  \              },\n              \"state\": {\n                \"type\": \"string\",\n                \"enum\": [\"Running\", \"Suspended\", \"Shutdown\", \"Overloaded\", \"Unknown\"]\n              },\n              \"enabled\": {\n                \"type\": \"boolean\"\n              },\n              \"activeConnectionsCurrentCount\": {\n                \"type\": \"integer\"\n              },\n              \"connectionsTotalCount\": {\n                \"type\": \"integer\"\n              },\n              \"currCapacity\": {\n                \"type\": \"integer\"\n              },\n              \"numAvailable\": {\n                \"type\": \"integer\"\n              },\n              \"numUnavailable\": {\n                \"type\": \"integer\"\n              },\n              \"waitingForConnectionCurrentCount\": {\n                \"type\": \"integer\"\n              },\n              \"leakedConnectionCount\": {\n                \"type\": \"integer\"\n              }\n         \
  \   }\n          }\n        }\n      }\n    },\n    \"JMSRuntime\": {\n      \"type\": \"object\",\n      \"description\": \"JMS runtime\",\n      \"properties\": {\n        \"connectionsCurrentCount\": {\n          \"type\": \"integer\"\n        },\n        \"connectionsTotalCount\": {\n          \"type\": \"integer\"\n        },\n        \"JMSServersCurrentCount\": {\n          \"type\": \"integer\"\n        },\n        \"healthState\": {\n          \"$ref\": \"#/$defs/HealthState\"\n        }\n      }\n    },\n    \"applicationRuntimes\": {\n      \"type\": \"array\",\n      \"description\": \"Runtime information for deployed applications\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"healthState\": {\n            \"$ref\": \"#/$defs/HealthState\"\n          },\n          \"overallHealthState\": {\n            \"$ref\": \"#/$defs/HealthState\"\n          }\n        }\n\
  \      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"HealthState\": {\n      \"type\": \"object\",\n      \"description\": \"Health state of a WebLogic Server component or subsystem\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Health state value\",\n          \"enum\": [\n            \"HEALTH_OK\",\n            \"HEALTH_WARN\",\n            \"HEALTH_CRITICAL\",\n            \"HEALTH_FAILED\",\n            \"HEALTH_OVERLOADED\"\n          ]\n        },\n        \"subsystemName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the subsystem reporting this health state\"\n        },\n        \"symptoms\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Symptoms or issues contributing to the health state\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/weblogic/refs/heads/main/json-schema/weblogic-server-runtime.json
tags:
- Application Server
- Enterprise
- Java EE
- Middleware
- Oracle
- WebLogic
title: WebLogic Server Runtime
---
