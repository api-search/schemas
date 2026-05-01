---
description: A member instance of a Neptune DB cluster.
layout: schema
name: DBClusterMember
properties_list:
- description: The instance identifier.
  name: DBInstanceIdentifier
  type: string
- description: Whether the instance is the primary (writer) instance.
  name: IsClusterWriter
  type: boolean
- description: The status of the parameter group for this member.
  name: DBClusterParameterGroupStatus
  type: string
- description: Failover priority for the instance.
  name: PromotionTier
  type: integer
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-db-cluster-member-schema.json
slug: management-db-cluster-member
source_filename: management-db-cluster-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-cluster-member-schema.json\",\n  \"title\": \"DBClusterMember\",\n  \"description\": \"A member instance of a Neptune DB cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBInstanceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The instance identifier.\"\n    },\n    \"IsClusterWriter\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the instance is the primary (writer) instance.\"\n    },\n    \"DBClusterParameterGroupStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the parameter group for this member.\"\n    },\n    \"PromotionTier\": {\n      \"type\": \"integer\",\n      \"description\": \"Failover priority for the instance.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-cluster-member-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DBClusterMember
---
