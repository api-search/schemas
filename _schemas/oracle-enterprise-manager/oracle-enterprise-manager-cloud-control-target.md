---
description: Represents a monitored target in Enterprise Manager. A target is any managed entity such as a database, host, middleware instance, or application.
layout: schema
name: Target
properties_list:
- description: Unique identifier of the target.
  name: targetId
  type: string
- description: Display name of the target.
  name: targetName
  type: string
- description: The type of the target, defining its monitoring template and available metrics.
  name: targetType
  type: string
- description: Human-readable target type display name.
  name: targetDisplayType
  type: string
- description: The hostname where the target resides.
  name: hostName
  type: string
- description: Current lifecycle status of the target.
  name: lifecycleStatus
  type: string
- description: Current availability status reported by monitoring.
  name: availabilityStatus
  type: string
- description: URL of the management agent monitoring this target.
  name: agentUrl
  type: string
- description: Oracle home directory path, applicable to Oracle targets.
  name: oracleHome
  type: string
- description: Machine name where the target is deployed.
  name: machineName
  type: string
- description: Installation directory path for the target software.
  name: installLocation
  type: string
- description: Time zone of the target.
  name: timezone
  type: string
- description: Enterprise Manager user who owns this target.
  name: owner
  type: string
- description: Timestamp when the target was added to Enterprise Manager.
  name: timeCreated
  type: string
- description: Timestamp of the last target configuration update.
  name: timeUpdated
  type: string
- description: Additional target-type-specific configuration properties.
  name: properties
  type: object
- description: Canonical URI for this target resource.
  name: canonicalLink
  type: string
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-target-schema.json
slug: oracle-enterprise-manager-cloud-control-target
source_filename: oracle-enterprise-manager-cloud-control-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Target\",\n  \"type\": \"object\",\n  \"description\": \"Represents a monitored target in Enterprise Manager. A target is any managed entity such as a database, host, middleware instance, or application.\",\n  \"properties\": {\n    \"targetId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the target.\"\n    },\n    \"targetName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the target.\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the target, defining its monitoring template and available metrics.\"\n    },\n    \"targetDisplayType\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable target type display name.\"\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname where the target resides.\"\n    },\n    \"lifecycleStatus\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the target.\"\n    },\n    \"availabilityStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current availability status reported by monitoring.\"\n    },\n    \"agentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the management agent monitoring this target.\"\n    },\n    \"oracleHome\": {\n      \"type\": \"string\",\n      \"description\": \"Oracle home directory path, applicable to Oracle targets.\"\n    },\n    \"machineName\": {\n      \"type\": \"string\",\n      \"description\": \"Machine name where the target is deployed.\"\n    },\n    \"installLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Installation directory path for the target software.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone of the target.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Enterprise Manager user who owns this target.\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the target was added to Enterprise Manager.\"\n    },\n    \"timeUpdated\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the last target configuration update.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Additional target-type-specific configuration properties.\"\n    },\n    \"canonicalLink\": {\n      \"type\": \"string\",\n      \"description\": \"Canonical URI for this target resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-target-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: Target
---
