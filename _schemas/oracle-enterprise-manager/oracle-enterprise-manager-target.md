---
description: Schema for a monitored target in Oracle Enterprise Manager Cloud Control. A target represents any managed entity such as an Oracle Database, host server, middleware instance, application, or composite system monitored through the Enterprise Manager platform.
layout: schema
name: Oracle Enterprise Manager Target
properties_list:
- description: Unique identifier assigned by Enterprise Manager when the target is registered.
  name: targetId
  type: string
- description: Display name of the target. Must be unique within the combination of target name and target type.
  name: targetName
  type: string
- description: The type of the target, defining its monitoring template, available metrics, and configuration properties.
  name: targetType
  type: string
- description: Human-readable display name for the target type.
  name: targetDisplayType
  type: string
- description: Fully qualified hostname or IP address where the target resides.
  name: hostName
  type: string
- description: Current lifecycle management status of the target within Enterprise Manager.
  name: lifecycleStatus
  type: string
- description: Current availability status as reported by the monitoring agent. Indicates whether the target is reachable and operational.
  name: availabilityStatus
  type: string
- description: URL of the Oracle Management Agent responsible for monitoring this target.
  name: agentUrl
  type: string
- description: Oracle home directory path on the target host. Applicable to Oracle software targets such as databases and middleware.
  name: oracleHome
  type: string
- description: Machine name where the target is deployed, which may differ from the hostname.
  name: machineName
  type: string
- description: Installation directory path for the target software.
  name: installLocation
  type: string
- description: Time zone of the target in standard timezone identifier format.
  name: timezone
  type: string
- description: Enterprise Manager username that owns this target and is responsible for its management.
  name: owner
  type: string
- description: ISO 8601 timestamp when the target was first added to Enterprise Manager.
  name: timeCreated
  type: string
- description: ISO 8601 timestamp of the most recent target configuration change.
  name: timeUpdated
  type: string
- description: Target-type-specific configuration and instance properties. The available properties vary based on the target type. Common examples include SID, port, service name, and version.
  name: properties
  type: object
- description: Global target properties used for classification, grouping, and organizational metadata.
  name: globalProperties
  type: object
- description: List of associations linking this target to other targets, such as cluster membership or composite relationships.
  name: associations
  type: array
- description: Canonical REST API URI for accessing this target resource.
  name: canonicalLink
  type: string
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-target-schema.json
slug: oracle-enterprise-manager-target
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://oracle.com/schemas/enterprise-manager/target.json\",\n  \"title\": \"Oracle Enterprise Manager Target\",\n  \"description\": \"Schema for a monitored target in Oracle Enterprise Manager Cloud Control. A target represents any managed entity such as an Oracle Database, host server, middleware instance, application, or composite system monitored through the Enterprise Manager platform.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"targetName\",\n    \"targetType\"\n  ],\n  \"properties\": {\n    \"targetId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by Enterprise Manager when the target is registered.\"\n    },\n    \"targetName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the target. Must be unique within the combination of target name and target type.\",\n      \"maxLength\": 256\n    },\n    \"targetType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The type of the target, defining its monitoring template, available metrics, and configuration properties.\",\n      \"examples\": [\n        \"oracle_database\",\n        \"host\",\n        \"weblogic_j2eeserver\",\n        \"oracle_pdb\",\n        \"rac_database\",\n        \"oracle_listener\",\n        \"oracle_emd\",\n        \"oracle_oms\",\n        \"j2ee_application\",\n        \"oracle_ias\",\n        \"oracle_apache\",\n        \"osm_instance\",\n        \"has\",\n        \"oracle_home\"\n      ]\n    },\n    \"targetDisplayType\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the target type.\",\n      \"examples\": [\n        \"Oracle Database\",\n        \"Host\",\n        \"Oracle WebLogic Server\",\n        \"Oracle Pluggable Database\",\n        \"Cluster Database\",\n        \"Oracle Listener\",\n        \"Oracle Management Agent\",\n        \"Oracle Management Service\"\
  \n      ]\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified hostname or IP address where the target resides.\",\n      \"maxLength\": 256\n    },\n    \"lifecycleStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle management status of the target within Enterprise Manager.\",\n      \"enum\": [\n        \"MONITORED\",\n        \"BLACKOUT\",\n        \"PENDING\",\n        \"DELETED\"\n      ]\n    },\n    \"availabilityStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current availability status as reported by the monitoring agent. Indicates whether the target is reachable and operational.\",\n      \"enum\": [\n        \"UP\",\n        \"DOWN\",\n        \"UNKNOWN\",\n        \"UNREACHABLE\",\n        \"BLACKOUT\",\n        \"NOT_MONITORED\",\n        \"ERROR\",\n        \"AGENT_UNREACHABLE\",\n        \"PENDING\"\n      ]\n    },\n    \"agentUrl\": {\n      \"type\": \"string\",\n      \"\
  format\": \"uri\",\n      \"description\": \"URL of the Oracle Management Agent responsible for monitoring this target.\"\n    },\n    \"oracleHome\": {\n      \"type\": \"string\",\n      \"description\": \"Oracle home directory path on the target host. Applicable to Oracle software targets such as databases and middleware.\",\n      \"examples\": [\n        \"/u01/app/oracle/product/19.0.0/dbhome_1\",\n        \"/u01/app/oracle/middleware\"\n      ]\n    },\n    \"machineName\": {\n      \"type\": \"string\",\n      \"description\": \"Machine name where the target is deployed, which may differ from the hostname.\"\n    },\n    \"installLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Installation directory path for the target software.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone of the target in standard timezone identifier format.\",\n      \"examples\": [\n        \"America/New_York\",\n        \"UTC\",\n     \
  \   \"Europe/London\"\n      ]\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Enterprise Manager username that owns this target and is responsible for its management.\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the target was first added to Enterprise Manager.\"\n    },\n    \"timeUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the most recent target configuration change.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Target-type-specific configuration and instance properties. The available properties vary based on the target type. Common examples include SID, port, service name, and version.\",\n      \"properties\": {\n        \"SID\": {\n          \"type\": \"string\",\n          \"description\": \"Oracle System Identifier for database\
  \ targets.\"\n        },\n        \"Port\": {\n          \"type\": \"string\",\n          \"description\": \"Listener or connection port number.\"\n        },\n        \"ServiceName\": {\n          \"type\": \"string\",\n          \"description\": \"Oracle database service name.\"\n        },\n        \"Version\": {\n          \"type\": \"string\",\n          \"description\": \"Software version of the target.\",\n          \"examples\": [\n            \"19.0.0.0.0\",\n            \"21.0.0.0.0\",\n            \"14.1.1.0.0\"\n          ]\n        },\n        \"Protocol\": {\n          \"type\": \"string\",\n          \"description\": \"Connection protocol used for monitoring.\",\n          \"enum\": [\n            \"TCP\",\n            \"TCPS\",\n            \"HTTP\",\n            \"HTTPS\"\n          ]\n        },\n        \"OracleHome\": {\n          \"type\": \"string\",\n          \"description\": \"Oracle home path as a target instance property.\"\n        },\n        \"MachineName\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Machine name as a target instance property.\"\n        },\n        \"RACOption\": {\n          \"type\": \"string\",\n          \"description\": \"Whether RAC is enabled for a database target.\",\n          \"enum\": [\n            \"YES\",\n            \"NO\"\n          ]\n        },\n        \"RoleSeparated\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the Oracle installation uses role separation.\",\n          \"enum\": [\n            \"YES\",\n            \"NO\"\n          ]\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"globalProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Global target properties used for classification, grouping, and organizational metadata.\",\n      \"properties\": {\n        \"orcl_gtp_lifecycle_status\": {\n          \"type\": \"string\",\n          \"description\": \"Lifecycle\
  \ stage of the target.\",\n          \"examples\": [\n            \"Production\",\n            \"Development\",\n            \"Staging\",\n            \"Test\"\n          ]\n        },\n        \"orcl_gtp_line_of_bus\": {\n          \"type\": \"string\",\n          \"description\": \"Line of business associated with the target.\"\n        },\n        \"orcl_gtp_cost_center\": {\n          \"type\": \"string\",\n          \"description\": \"Cost center associated with the target.\"\n        },\n        \"orcl_gtp_department\": {\n          \"type\": \"string\",\n          \"description\": \"Department responsible for the target.\"\n        },\n        \"orcl_gtp_location\": {\n          \"type\": \"string\",\n          \"description\": \"Physical or logical location of the target.\"\n        },\n        \"orcl_gtp_contact\": {\n          \"type\": \"string\",\n          \"description\": \"Contact person for the target.\"\n        },\n        \"orcl_gtp_comment\": {\n          \"type\":\
  \ \"string\",\n          \"description\": \"Free-form comment about the target.\"\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"associations\": {\n      \"type\": \"array\",\n      \"description\": \"List of associations linking this target to other targets, such as cluster membership or composite relationships.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"associationType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of association.\",\n            \"examples\": [\n              \"contains\",\n              \"hosted_by\",\n              \"runs_on\",\n              \"member_of\",\n              \"monitored_by\"\n            ]\n          },\n          \"targetName\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the associated target.\"\n          },\n          \"targetType\": {\n            \"type\": \"string\",\n\
  \            \"description\": \"Type of the associated target.\"\n          }\n        }\n      }\n    },\n    \"canonicalLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Canonical REST API URI for accessing this target resource.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-target-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: Oracle Enterprise Manager Target
---
