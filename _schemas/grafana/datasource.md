---
description: Schema for a Grafana data source configuration, defining connection details and type-specific settings for backends such as Prometheus, MySQL, Elasticsearch, Loki, and others.
layout: schema
name: Grafana Data Source Configuration
properties_list:
- description: Auto-generated numeric ID
  name: id
  type: integer
- description: Unique identifier that can be set by the client for stable cross-instance references
  name: uid
  type: string
- description: Organization ID the data source belongs to
  name: orgId
  type: integer
- description: Human-readable name, must be unique within the org
  name: name
  type: string
- description: Data source plugin type identifier
  name: type
  type: string
- description: 'Access mode: proxy (server-side) or direct (browser-side, deprecated)'
  name: access
  type: string
- description: URL of the data source backend
  name: url
  type: string
- description: Username for data source authentication
  name: user
  type: string
- description: Default database name
  name: database
  type: string
- description: Whether basic auth is enabled for the data source connection
  name: basicAuth
  type: boolean
- description: Basic auth username
  name: basicAuthUser
  type: string
- description: Whether to send credentials (cookies, auth headers) with cross-site requests
  name: withCredentials
  type: boolean
- description: Whether this is the default data source for the organization
  name: isDefault
  type: boolean
- description: Whether the data source was provisioned and cannot be modified via the UI
  name: readOnly
  type: boolean
- description: Version number for optimistic locking
  name: version
  type: integer
- description: Data-source-type-specific configuration stored as JSON
  name: jsonData
  type: object
- description: Sensitive configuration fields (passwords, tokens) - write-only, never returned by the API
  name: secureJsonData
  type: object
- description: Indicates which secure fields are set (returned by GET). Keys are field names, values are boolean true.
  name: secureJsonFields
  type: object
provider_name: Grafana
provider_slug: grafana
schema_file: json-schema/datasource.json
slug: datasource
source_filename: datasource.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/grafana/json-schema/datasource.json\",\n  \"title\": \"Grafana Data Source Configuration\",\n  \"description\": \"Schema for a Grafana data source configuration, defining connection details and type-specific settings for backends such as Prometheus, MySQL, Elasticsearch, Loki, and others.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Auto-generated numeric ID\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier that can be set by the client for stable cross-instance references\",\n      \"maxLength\": 40\n    },\n    \"orgId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization ID the data source belongs to\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name, must be unique\
  \ within the org\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Data source plugin type identifier\",\n      \"examples\": [\n        \"prometheus\", \"loki\", \"elasticsearch\", \"mysql\", \"postgres\",\n        \"mssql\", \"influxdb\", \"graphite\", \"cloudwatch\", \"stackdriver\",\n        \"azure-monitor\", \"tempo\", \"jaeger\", \"zipkin\", \"opentsdb\",\n        \"testdata\", \"grafana-pyroscope-datasource\"\n      ]\n    },\n    \"access\": {\n      \"type\": \"string\",\n      \"enum\": [\"proxy\", \"direct\"],\n      \"default\": \"proxy\",\n      \"description\": \"Access mode: proxy (server-side) or direct (browser-side, deprecated)\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the data source backend\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Username for data source authentication\"\n    },\n    \"database\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Default database name\"\n    },\n    \"basicAuth\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether basic auth is enabled for the data source connection\"\n    },\n    \"basicAuthUser\": {\n      \"type\": \"string\",\n      \"description\": \"Basic auth username\"\n    },\n    \"withCredentials\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to send credentials (cookies, auth headers) with cross-site requests\"\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether this is the default data source for the organization\"\n    },\n    \"readOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the data source was provisioned and cannot be modified via the UI\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number for optimistic locking\"\
  \n    },\n    \"jsonData\": {\n      \"type\": \"object\",\n      \"description\": \"Data-source-type-specific configuration stored as JSON\",\n      \"properties\": {\n        \"httpMethod\": {\n          \"type\": \"string\",\n          \"enum\": [\"GET\", \"POST\"],\n          \"description\": \"HTTP method for queries (Prometheus)\"\n        },\n        \"timeInterval\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum scrape interval (Prometheus)\"\n        },\n        \"queryTimeout\": {\n          \"type\": \"string\",\n          \"description\": \"Query timeout\"\n        },\n        \"tlsAuth\": { \"type\": \"boolean\" },\n        \"tlsAuthWithCACert\": { \"type\": \"boolean\" },\n        \"tlsSkipVerify\": { \"type\": \"boolean\" },\n        \"oauthPassThru\": { \"type\": \"boolean\" },\n        \"timeout\": { \"type\": \"integer\" },\n        \"esVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Elasticsearch version\"\n    \
  \    },\n        \"timeField\": {\n          \"type\": \"string\",\n          \"description\": \"Default time field (Elasticsearch)\"\n        },\n        \"maxConcurrentShardRequests\": {\n          \"type\": \"integer\",\n          \"description\": \"Max concurrent shard requests (Elasticsearch)\"\n        },\n        \"logMessageField\": {\n          \"type\": \"string\",\n          \"description\": \"Log message field name (Elasticsearch)\"\n        },\n        \"logLevelField\": {\n          \"type\": \"string\",\n          \"description\": \"Log level field name (Elasticsearch)\"\n        },\n        \"derivedFields\": {\n          \"type\": \"array\",\n          \"description\": \"Derived fields for Loki\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"matcherRegex\": { \"type\": \"string\" },\n              \"url\": { \"type\": \"string\" },\n              \"datasourceUid\"\
  : { \"type\": \"string\" }\n            }\n          }\n        },\n        \"maxLines\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum log lines to return (Loki)\"\n        },\n        \"tracesToLogs\": {\n          \"type\": \"object\",\n          \"description\": \"Trace to logs correlation settings\"\n        },\n        \"serviceMap\": {\n          \"type\": \"object\",\n          \"description\": \"Service map settings (Tempo)\"\n        },\n        \"nodeGraph\": {\n          \"type\": \"object\",\n          \"description\": \"Node graph settings\"\n        },\n        \"alertmanagerUid\": {\n          \"type\": \"string\"\n        },\n        \"manageAlerts\": {\n          \"type\": \"boolean\"\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"secureJsonData\": {\n      \"type\": \"object\",\n      \"description\": \"Sensitive configuration fields (passwords, tokens) - write-only, never returned by the API\",\n      \"properties\"\
  : {\n        \"password\": { \"type\": \"string\" },\n        \"basicAuthPassword\": { \"type\": \"string\" },\n        \"tlsCACert\": { \"type\": \"string\" },\n        \"tlsClientCert\": { \"type\": \"string\" },\n        \"tlsClientKey\": { \"type\": \"string\" },\n        \"accessKey\": { \"type\": \"string\" },\n        \"secretKey\": { \"type\": \"string\" },\n        \"httpHeaderValue1\": { \"type\": \"string\" }\n      },\n      \"additionalProperties\": true\n    },\n    \"secureJsonFields\": {\n      \"type\": \"object\",\n      \"description\": \"Indicates which secure fields are set (returned by GET). Keys are field names, values are boolean true.\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      }\n    }\n  },\n  \"required\": [\"name\", \"type\", \"access\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grafana/refs/heads/main/json-schema/datasource.json
tags:
- Alerting
- Analytics
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
- Traces
- Visualization
title: Grafana Data Source Configuration
---
