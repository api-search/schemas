---
description: Schema for configuring a Pixie plugin that exports observability data from Pixie at scheduled intervals to external systems. Plugins pair PxL export scripts with a retention plugin backend such as an OpenTelemetry collector or Grafana datasource.
layout: schema
name: Pixie Plugin Configuration
properties_list:
- description: Unique identifier of the plugin to configure, such as 'grafana' or 'open-telemetry'.
  name: plugin_id
  type: string
- description: Whether the plugin is enabled for this cluster.
  name: enabled
  type: boolean
- description: Version of the plugin to use.
  name: version
  type: string
- description: JSON-encoded plugin-specific configuration. Contents vary by plugin type. For OpenTelemetry, this includes the collector endpoint; for Grafana, the datasource URL.
  name: config_json
  type: string
- description: Custom URL for exporting data when using a self-hosted or custom endpoint.
  name: customExportURL
  type: string
- description: If true, TLS certificate validation is skipped when connecting to the export endpoint. Not recommended for production.
  name: insecureTLS
  type: boolean
- description: List of PxL retention script configurations defining what data to export and at what frequency.
  name: retention_scripts
  type: array
provider_name: Pixie
provider_slug: pixie
schema_file: json-schema/pixie-plugin-schema.json
slug: pixie-plugin
source_filename: pixie-plugin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.px.dev/schemas/plugin.json\",\n  \"title\": \"Pixie Plugin Configuration\",\n  \"description\": \"Schema for configuring a Pixie plugin that exports observability data from Pixie at scheduled intervals to external systems. Plugins pair PxL export scripts with a retention plugin backend such as an OpenTelemetry collector or Grafana datasource.\",\n  \"type\": \"object\",\n  \"required\": [\"plugin_id\", \"enabled\"],\n  \"properties\": {\n    \"plugin_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the plugin to configure, such as 'grafana' or 'open-telemetry'.\",\n      \"examples\": [\"grafana\", \"open-telemetry\", \"datadog\", \"newrelic\"]\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the plugin is enabled for this cluster.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Version of the plugin to use.\"\n    },\n    \"config_json\": {\n      \"type\": \"string\",\n      \"description\": \"JSON-encoded plugin-specific configuration. Contents vary by plugin type. For OpenTelemetry, this includes the collector endpoint; for Grafana, the datasource URL.\"\n    },\n    \"customExportURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Custom URL for exporting data when using a self-hosted or custom endpoint.\"\n    },\n    \"insecureTLS\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, TLS certificate validation is skipped when connecting to the export endpoint. Not recommended for production.\"\n    },\n    \"retention_scripts\": {\n      \"type\": \"array\",\n      \"description\": \"List of PxL retention script configurations defining what data to export and at what frequency.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RetentionScript\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"RetentionScript\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Configuration for a PxL script that periodically exports Pixie telemetry data to the plugin backend.\",\n      \"required\": [\"script_name\", \"script\", \"frequency_s\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier of the retention script.\"\n        },\n        \"script_name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name of the retention script.\",\n          \"maxLength\": 200\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of what data this script exports.\"\n        },\n        \"script\": {\n          \"type\": \"string\",\n          \"description\": \"PxL source code for the export script. The script should use px.export() to send data to the configured plugin endpoint rather than px.display().\",\n  \
  \        \"minLength\": 1\n        },\n        \"frequency_s\": {\n          \"type\": \"integer\",\n          \"description\": \"How often the script is executed in seconds. Controls the export cadence for this data stream.\",\n          \"minimum\": 10,\n          \"maximum\": 86400\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this retention script is active and exporting data.\"\n        },\n        \"cluster_ids\": {\n          \"type\": \"array\",\n          \"description\": \"List of cluster IDs to run this script on. If empty, the script runs on all clusters.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          }\n        },\n        \"plugin_id\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the plugin this script exports data to.\"\n        },\n        \"export_url\": {\n          \"type\": \"string\",\n          \"format\": \"\
  uri\",\n          \"description\": \"Endpoint URL where the script sends exported data.\"\n        },\n        \"custom_export_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Override export URL for this specific script.\"\n        },\n        \"is_preset\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, this script is a built-in preset provided by the plugin, not a user-defined script.\"\n        }\n      }\n    },\n    \"OpenTelemetryConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for the OpenTelemetry export plugin.\",\n      \"required\": [\"endpoint\"],\n      \"properties\": {\n        \"endpoint\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"OTLP gRPC or HTTP endpoint for sending telemetry data.\"\n        },\n        \"headers\": {\n          \"type\": \"object\",\n          \"description\": \"Additional HTTP headers\
  \ to include with export requests, such as authentication tokens.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"insecure\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, sends data over an unencrypted connection.\"\n        }\n      }\n    },\n    \"GrafanaConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for the Grafana plugin that exposes Pixie data as a Grafana datasource.\",\n      \"properties\": {\n        \"grafana_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the Grafana instance to connect to.\"\n        },\n        \"grafana_api_key\": {\n          \"type\": \"string\",\n          \"description\": \"Grafana API key with datasource write permission.\"\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"plugin_id\": \"open-telemetry\",\n      \"enabled\": true,\n      \"version\"\
  : \"1.0\",\n      \"retention_scripts\": [\n        {\n          \"script_name\": \"HTTP Metrics Export\",\n          \"description\": \"Exports HTTP request metrics to OpenTelemetry collector every 60 seconds.\",\n          \"script\": \"import px\\nimport pxtrace\\n# Export HTTP events\\ndf = px.DataFrame(table='http_events', start_time=px.plugin.start_time)\\ndf.service = df.ctx['service']\\npx.export(df, px.otel.Data(resource=px.otel.Resource(attrs={'service.name': df.service}), data=[px.otel.metric.Gauge(name='http.resp_latency', value=df.resp_latency_ns)]))\",\n          \"frequency_s\": 60,\n          \"enabled\": true\n        }\n      ]\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pixie/refs/heads/main/json-schema/pixie-plugin-schema.json
tags:
- eBPF
- Kubernetes
- Monitoring
- Observability
title: Pixie Plugin Configuration
---
