---
description: Schema for a Grafana panel within a dashboard, defining visualization type, queries, field configuration, and layout position.
layout: schema
name: Grafana Panel
properties_list:
- description: Unique numeric ID within the dashboard
  name: id
  type: integer
- description: Panel visualization plugin type
  name: type
  type: string
- description: Panel title displayed in the header
  name: title
  type: string
- description: Panel description, shown on hover over the info icon
  name: description
  type: string
- description: Whether to display the panel without a background
  name: transparent
  type: boolean
- description: Panel position and size on the dashboard grid (24 columns wide)
  name: gridPos
  type: object
- description: Default data source for this panel
  name: datasource
  type:
  - object
  - 'null'
- description: Query targets - structure varies by data source type
  name: targets
  type: array
- description: Field display configuration
  name: fieldConfig
  type: object
- description: Panel-type-specific visualization options. Structure depends on the panel type.
  name: options
  type: object
- description: Data transformations applied before visualization
  name: transformations
  type: array
- description: Template variable name to repeat this panel for each value
  name: repeat
  type: string
- description: 'Direction to repeat panels: h (horizontal) or v (vertical)'
  name: repeatDirection
  type: string
- description: Maximum number of panels per row when repeating horizontally
  name: maxPerRow
  type: integer
- description: Panel-level links
  name: links
  type: array
- description: Legacy alerting rule attached to the panel (deprecated in favor of unified alerting)
  name: alert
  type: object
- description: Only for row panels - whether the row is collapsed
  name: collapsed
  type: boolean
- description: Only for row panels - nested panels within a collapsed row
  name: panels
  type: array
provider_name: Grafana
provider_slug: grafana
schema_file: json-schema/panel.json
slug: panel
source_filename: panel.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/grafana/json-schema/panel.json\",\n  \"title\": \"Grafana Panel\",\n  \"description\": \"Schema for a Grafana panel within a dashboard, defining visualization type, queries, field configuration, and layout position.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric ID within the dashboard\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Panel visualization plugin type\",\n      \"examples\": [\n        \"timeseries\", \"stat\", \"gauge\", \"bargauge\", \"table\",\n        \"barchart\", \"piechart\", \"histogram\", \"heatmap\", \"state-timeline\",\n        \"status-history\", \"text\", \"logs\", \"nodeGraph\", \"traces\",\n        \"flamegraph\", \"geomap\", \"canvas\", \"candlestick\", \"trend\",\n        \"news\", \"dashlist\", \"alertlist\", \"\
  annolist\", \"row\"\n      ]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Panel title displayed in the header\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Panel description, shown on hover over the info icon\"\n    },\n    \"transparent\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to display the panel without a background\"\n    },\n    \"gridPos\": {\n      \"type\": \"object\",\n      \"description\": \"Panel position and size on the dashboard grid (24 columns wide)\",\n      \"properties\": {\n        \"h\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Panel height in grid units\"\n        },\n        \"w\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 24,\n          \"description\": \"Panel width in grid units (max 24)\"\n        },\n        \"x\": {\n          \"\
  type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 23,\n          \"description\": \"Panel x position (column)\"\n        },\n        \"y\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Panel y position (row)\"\n        }\n      },\n      \"required\": [\"h\", \"w\", \"x\", \"y\"]\n    },\n    \"datasource\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Default data source for this panel\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Data source plugin type\"\n        },\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"Data source UID\"\n        }\n      }\n    },\n    \"targets\": {\n      \"type\": \"array\",\n      \"description\": \"Query targets - structure varies by data source type\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"refId\": {\n   \
  \         \"type\": \"string\",\n            \"description\": \"Reference ID for the query (A, B, C, ...)\"\n          },\n          \"datasource\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": { \"type\": \"string\" },\n              \"uid\": { \"type\": \"string\" }\n            }\n          },\n          \"expr\": {\n            \"type\": \"string\",\n            \"description\": \"PromQL expression (Prometheus/Mimir/Thanos)\"\n          },\n          \"rawSql\": {\n            \"type\": \"string\",\n            \"description\": \"Raw SQL query (MySQL, PostgreSQL, MSSQL)\"\n          },\n          \"query\": {\n            \"type\": \"string\",\n            \"description\": \"Generic query field (Loki LogQL, Elasticsearch, etc.)\"\n          },\n          \"format\": {\n            \"type\": \"string\",\n            \"description\": \"Response format\"\n          },\n          \"legendFormat\": {\n            \"type\": \"string\",\n  \
  \          \"description\": \"Legend label template\"\n          },\n          \"interval\": {\n            \"type\": \"string\",\n            \"description\": \"Minimum step interval\"\n          },\n          \"instant\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether to execute as an instant query\"\n          },\n          \"range\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether to execute as a range query\"\n          },\n          \"hide\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether to hide this query from visualization\"\n          },\n          \"editorMode\": {\n            \"type\": \"string\",\n            \"enum\": [\"code\", \"builder\"]\n          }\n        },\n        \"required\": [\"refId\"]\n      }\n    },\n    \"fieldConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Field display configuration\",\n      \"properties\": {\n        \"defaults\": {\n    \
  \      \"type\": \"object\",\n          \"properties\": {\n            \"unit\": {\n              \"type\": \"string\",\n              \"description\": \"Unit of measurement, e.g. bytes, percent, s, ms, reqps\"\n            },\n            \"min\": { \"type\": \"number\" },\n            \"max\": { \"type\": \"number\" },\n            \"decimals\": { \"type\": \"integer\" },\n            \"displayName\": { \"type\": \"string\" },\n            \"noValue\": { \"type\": \"string\" },\n            \"color\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"mode\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"palette-classic\", \"fixed\", \"continuous-GrYlRd\", \"continuous-BlYlRd\", \"continuous-blues\", \"continuous-reds\", \"continuous-greens\", \"continuous-purples\", \"shades\"]\n                },\n                \"fixedColor\": { \"type\": \"string\" }\n              }\n            },\n            \"thresholds\"\
  : {\n              \"type\": \"object\",\n              \"properties\": {\n                \"mode\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"absolute\", \"percentage\"]\n                },\n                \"steps\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"color\": { \"type\": \"string\" },\n                      \"value\": { \"type\": [\"number\", \"null\"] }\n                    },\n                    \"required\": [\"color\", \"value\"]\n                  }\n                }\n              }\n            },\n            \"mappings\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"enum\": [\"value\", \"range\", \"regex\",\
  \ \"special\"]\n                  },\n                  \"options\": { \"type\": \"object\" }\n                }\n              }\n            },\n            \"links\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"object\" }\n            },\n            \"custom\": {\n              \"type\": \"object\",\n              \"description\": \"Panel-type-specific field configuration\"\n            }\n          }\n        },\n        \"overrides\": {\n          \"type\": \"array\",\n          \"description\": \"Field-specific overrides\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"matcher\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"enum\": [\"byName\", \"byRegexp\", \"byType\", \"byFrameRefID\"]\n                  },\n                  \"options\": {}\n                }\n\
  \              },\n              \"properties\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"id\": { \"type\": \"string\" },\n                    \"value\": {}\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"Panel-type-specific visualization options. Structure depends on the panel type.\"\n    },\n    \"transformations\": {\n      \"type\": \"array\",\n      \"description\": \"Data transformations applied before visualization\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Transformation type, e.g. merge, organize, filterFieldsByName, reduce, groupBy, joinByField, calculateField, sortBy\"\n          },\n\
  \          \"options\": {\n            \"type\": \"object\",\n            \"description\": \"Transformation-specific options\"\n          },\n          \"disabled\": {\n            \"type\": \"boolean\"\n          },\n          \"filter\": {\n            \"type\": \"object\"\n          }\n        },\n        \"required\": [\"id\", \"options\"]\n      }\n    },\n    \"repeat\": {\n      \"type\": \"string\",\n      \"description\": \"Template variable name to repeat this panel for each value\"\n    },\n    \"repeatDirection\": {\n      \"type\": \"string\",\n      \"enum\": [\"h\", \"v\"],\n      \"description\": \"Direction to repeat panels: h (horizontal) or v (vertical)\"\n    },\n    \"maxPerRow\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of panels per row when repeating horizontally\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"Panel-level links\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"title\": { \"type\": \"string\" },\n          \"url\": { \"type\": \"string\" },\n          \"targetBlank\": { \"type\": \"boolean\" }\n        }\n      }\n    },\n    \"alert\": {\n      \"type\": \"object\",\n      \"description\": \"Legacy alerting rule attached to the panel (deprecated in favor of unified alerting)\"\n    },\n    \"collapsed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Only for row panels - whether the row is collapsed\"\n    },\n    \"panels\": {\n      \"type\": \"array\",\n      \"description\": \"Only for row panels - nested panels within a collapsed row\",\n      \"items\": { \"$ref\": \"#\" }\n    }\n  },\n  \"required\": [\"type\", \"gridPos\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grafana/refs/heads/main/json-schema/panel.json
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
title: Grafana Panel
---
