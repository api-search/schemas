---
description: Cluster setup status
layout: schema
name: ClusterSetupResponse
properties_list:
- description: Cluster setup state
  name: state
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-cluster-setup-response-schema.json
slug: apache-couchdb-cluster-setup-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-cluster-setup-response-schema.json\",\n  \"title\": \"ClusterSetupResponse\",\n  \"description\": \"Cluster setup status\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster setup state\",\n      \"enum\": [\n        \"cluster_disabled\",\n        \"single_node_disabled\",\n        \"single_node_enabled\",\n        \"cluster_enabled\",\n        \"cluster_finished\"\n      ],\n      \"example\": \"cluster_enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-cluster-setup-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ClusterSetupResponse
---
