---
description: Schema for the Chart.yaml file that describes a Helm chart. Chart.yaml contains metadata about the chart including its name, version, dependencies, and maintainers. This file is required in every Helm chart.
layout: schema
name: Helm Chart.yaml
properties_list:
- description: The chart API version. v2 is for Helm 3 charts, v1 is for Helm 2 charts.
  name: apiVersion
  type: string
- description: The name of the chart. Must match the directory name.
  name: name
  type: string
- description: The SemVer 2 version of the chart. This is used as a release marker and must be incremented for each new release.
  name: version
  type: string
- description: A SemVer range of compatible Kubernetes versions. Helm validates this constraint during installation.
  name: kubeVersion
  type: string
- description: A single-sentence description of the chart.
  name: description
  type: string
- description: The type of the chart. Application charts are installable, library charts provide utilities for other charts.
  name: type
  type: string
- description: A list of keywords associated with the chart for search and categorization.
  name: keywords
  type: array
- description: The URL of the project home page.
  name: home
  type: string
- description: A list of URLs to source code for this chart.
  name: sources
  type: array
- description: A list of chart dependencies. Helm downloads these charts into the charts/ directory during dependency resolution.
  name: dependencies
  type: array
- description: A list of chart maintainers with contact information.
  name: maintainers
  type: array
- description: A URL to an SVG or PNG icon to display in the Helm UI and artifact hub.
  name: icon
  type: string
- description: The version of the application that the chart deploys. This is informational and does not affect chart version calculations.
  name: appVersion
  type: string
- description: Whether this chart is deprecated. When set to true, Helm shows a warning during installation.
  name: deprecated
  type: boolean
- description: Annotations are key-value pairs used by Artifact Hub and other tools to store additional metadata.
  name: annotations
  type: object
provider_name: Helm
provider_slug: helm
schema_file: json-schema/helm-chart-yaml-schema.json
slug: helm-chart-yaml
source_filename: helm-chart-yaml-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://helm.sh/schemas/chart-yaml.json\",\n  \"title\": \"Helm Chart.yaml\",\n  \"description\": \"Schema for the Chart.yaml file that describes a Helm chart. Chart.yaml contains metadata about the chart including its name, version, dependencies, and maintainers. This file is required in every Helm chart.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"apiVersion\",\n    \"name\",\n    \"version\"\n  ],\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The chart API version. v2 is for Helm 3 charts, v1 is for Helm 2 charts.\",\n      \"enum\": [\n        \"v1\",\n        \"v2\"\n      ],\n      \"default\": \"v2\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the chart. Must match the directory name.\",\n      \"pattern\": \"^[a-zA-Z0-9][a-zA-Z0-9._-]*$\",\n      \"examples\": [\n        \"nginx\"\
  ,\n        \"my-application\"\n      ]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The SemVer 2 version of the chart. This is used as a release marker and must be incremented for each new release.\",\n      \"pattern\": \"^(0|[1-9]\\\\d*)\\\\.(0|[1-9]\\\\d*)\\\\.(0|[1-9]\\\\d*)(-[\\\\da-zA-Z-]+(\\\\.[\\\\da-zA-Z-]+)*)?(\\\\+[\\\\da-zA-Z-]+(\\\\.[\\\\da-zA-Z-]+)*)?$\",\n      \"examples\": [\n        \"1.0.0\",\n        \"2.1.3-beta.1\"\n      ]\n    },\n    \"kubeVersion\": {\n      \"type\": \"string\",\n      \"description\": \"A SemVer range of compatible Kubernetes versions. Helm validates this constraint during installation.\",\n      \"examples\": [\n        \">= 1.19.0\",\n        \">= 1.20.0-0 < 1.28.0-0\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A single-sentence description of the chart.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the\
  \ chart. Application charts are installable, library charts provide utilities for other charts.\",\n      \"enum\": [\n        \"application\",\n        \"library\"\n      ],\n      \"default\": \"application\"\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"description\": \"A list of keywords associated with the chart for search and categorization.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"nginx\", \"web server\", \"proxy\"]\n      ]\n    },\n    \"home\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the project home page.\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"description\": \"A list of URLs to source code for this chart.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"A list of chart dependencies. Helm downloads\
  \ these charts into the charts/ directory during dependency resolution.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Dependency\"\n      }\n    },\n    \"maintainers\": {\n      \"type\": \"array\",\n      \"description\": \"A list of chart maintainers with contact information.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Maintainer\"\n      }\n    },\n    \"icon\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to an SVG or PNG icon to display in the Helm UI and artifact hub.\"\n    },\n    \"appVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the application that the chart deploys. This is informational and does not affect chart version calculations.\",\n      \"examples\": [\n        \"1.21.0\",\n        \"8.0.28\"\n      ]\n    },\n    \"deprecated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this chart is deprecated. When set to true, Helm shows a warning during installation.\"\
  ,\n      \"default\": false\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"description\": \"Annotations are key-value pairs used by Artifact Hub and other tools to store additional metadata.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        {\n          \"artifacthub.io/category\": \"networking\",\n          \"artifacthub.io/license\": \"Apache-2.0\"\n        }\n      ]\n    }\n  },\n  \"$defs\": {\n    \"Dependency\": {\n      \"type\": \"object\",\n      \"description\": \"A chart dependency specifying another chart that must be present in the charts/ directory.\",\n      \"required\": [\n        \"name\",\n        \"version\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the dependency chart.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The SemVer range for the dependency\
  \ version.\"\n        },\n        \"repository\": {\n          \"type\": \"string\",\n          \"description\": \"The URL of the chart repository where the dependency is hosted. Can also use the alias:// prefix for named repositories.\",\n          \"examples\": [\n            \"https://charts.bitnami.com/bitnami\",\n            \"alias://my-repo\"\n          ]\n        },\n        \"condition\": {\n          \"type\": \"string\",\n          \"description\": \"A YAML path in the parent chart's values that resolves to a boolean, controlling whether this dependency is enabled.\",\n          \"examples\": [\n            \"redis.enabled\",\n            \"global.redis.enabled\"\n          ]\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"description\": \"Tags used to group chart dependencies together for bulk enable/disable.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"import-values\": {\n          \"description\"\
  : \"Mapping of values to import from the child chart into the parent chart's values.\",\n          \"oneOf\": [\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"child\": {\n                    \"type\": \"string\"\n                  },\n                  \"parent\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          ]\n        },\n        \"alias\": {\n          \"type\": \"string\",\n          \"description\": \"An alias name for the dependency, allowing the same chart to be used multiple times with different configurations.\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the dependency\
  \ is enabled by default.\",\n          \"default\": true\n        }\n      }\n    },\n    \"Maintainer\": {\n      \"type\": \"object\",\n      \"description\": \"Contact information for a chart maintainer.\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The maintainer's name.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The maintainer's email address.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The maintainer's personal or organizational URL.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/helm/refs/heads/main/json-schema/helm-chart-yaml-schema.json
tags:
- Charts
- Cloud Native
- Container Orchestration
- DevOps
- Kubernetes
- Package Manager
title: Helm Chart.yaml
---
