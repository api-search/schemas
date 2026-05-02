---
description: Schema for the plugin.yaml file that describes a Helm CLI plugin. The plugin.yaml file defines the plugin's name, version, command to execute, hooks, and platform-specific binaries. Helm plugins are installed into a single directory and extend the Helm CLI with additional subcommands.
layout: schema
name: Helm Plugin Descriptor
properties_list:
- description: The name of the plugin. This becomes the subcommand name (e.g., 'helm name'). Must be lowercase letters, numbers, and hyphens.
  name: name
  type: string
- description: The SemVer 2 version of the plugin.
  name: version
  type: string
- description: A short usage description shown in the 'helm help' output and 'helm plugin list' command.
  name: usage
  type: string
- description: A longer description of the plugin's functionality shown in 'helm <plugin> --help'.
  name: description
  type: string
- description: The command to run when the plugin is invoked. Can reference the plugin directory with $HELM_PLUGIN_DIR. On Windows, use a batch file path.
  name: command
  type: string
- description: When true, Helm will not pass global flags to the plugin command. Useful for plugins that handle their own flag parsing.
  name: ignoreFlags
  type: boolean
- description: Deprecated in Helm 3. Previously used to create a tunnel to Tiller. Has no effect in Helm 3.
  name: useTunnel
  type: boolean
- description: ''
  name: hooks
  type: object
- description: Custom protocol downloaders provided by this plugin. Allows the plugin to handle custom repository URL schemes.
  name: downloaders
  type: array
- description: Platform-specific command overrides. Helm selects the matching entry based on the current OS and architecture.
  name: platformCommand
  type: array
provider_name: Helm
provider_slug: helm
schema_file: json-schema/helm-plugin-schema.json
slug: helm-plugin
source_filename: helm-plugin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://helm.sh/schemas/plugin.json\",\n  \"title\": \"Helm Plugin Descriptor\",\n  \"description\": \"Schema for the plugin.yaml file that describes a Helm CLI plugin. The plugin.yaml file defines the plugin's name, version, command to execute, hooks, and platform-specific binaries. Helm plugins are installed into a single directory and extend the Helm CLI with additional subcommands.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"version\",\n    \"usage\",\n    \"description\",\n    \"command\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the plugin. This becomes the subcommand name (e.g., 'helm name'). Must be lowercase letters, numbers, and hyphens.\",\n      \"pattern\": \"^[a-z][a-z0-9-]*$\",\n      \"examples\": [\n        \"diff\",\n        \"secrets\",\n        \"push\"\n      ]\n    },\n    \"version\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The SemVer 2 version of the plugin.\",\n      \"pattern\": \"^(0|[1-9]\\\\d*)\\\\.(0|[1-9]\\\\d*)\\\\.(0|[1-9]\\\\d*)(-[\\\\da-zA-Z-]+(\\\\.[\\\\da-zA-Z-]+)*)?(\\\\+[\\\\da-zA-Z-]+(\\\\.[\\\\da-zA-Z-]+)*)?$\",\n      \"examples\": [\n        \"3.9.0\",\n        \"1.0.0-beta.1\"\n      ]\n    },\n    \"usage\": {\n      \"type\": \"string\",\n      \"description\": \"A short usage description shown in the 'helm help' output and 'helm plugin list' command.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A longer description of the plugin's functionality shown in 'helm <plugin> --help'.\"\n    },\n    \"command\": {\n      \"type\": \"string\",\n      \"description\": \"The command to run when the plugin is invoked. Can reference the plugin directory with $HELM_PLUGIN_DIR. On Windows, use a batch file path.\",\n      \"examples\": [\n        \"$HELM_PLUGIN_DIR/bin/helm-diff\",\n        \"sh\
  \ $HELM_PLUGIN_DIR/plugin.sh\"\n      ]\n    },\n    \"ignoreFlags\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, Helm will not pass global flags to the plugin command. Useful for plugins that handle their own flag parsing.\",\n      \"default\": false\n    },\n    \"useTunnel\": {\n      \"type\": \"boolean\",\n      \"description\": \"Deprecated in Helm 3. Previously used to create a tunnel to Tiller. Has no effect in Helm 3.\",\n      \"default\": false\n    },\n    \"hooks\": {\n      \"$ref\": \"#/$defs/Hooks\"\n    },\n    \"downloaders\": {\n      \"type\": \"array\",\n      \"description\": \"Custom protocol downloaders provided by this plugin. Allows the plugin to handle custom repository URL schemes.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Downloader\"\n      }\n    },\n    \"platformCommand\": {\n      \"type\": \"array\",\n      \"description\": \"Platform-specific command overrides. Helm selects the matching entry based on the current OS\
  \ and architecture.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PlatformCommand\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Hooks\": {\n      \"type\": \"object\",\n      \"description\": \"Lifecycle hooks for the plugin. Hooks run shell commands at defined points in the plugin lifecycle.\",\n      \"properties\": {\n        \"install\": {\n          \"type\": \"string\",\n          \"description\": \"Shell command to run when the plugin is installed with 'helm plugin install'.\",\n          \"examples\": [\n            \"bash install.sh\"\n          ]\n        },\n        \"update\": {\n          \"type\": \"string\",\n          \"description\": \"Shell command to run when the plugin is updated with 'helm plugin update'.\",\n          \"examples\": [\n            \"bash install.sh\"\n          ]\n        },\n        \"delete\": {\n          \"type\": \"string\",\n          \"description\": \"Shell command to run when the plugin is removed with 'helm plugin uninstall'.\"\n \
  \       }\n      }\n    },\n    \"Downloader\": {\n      \"type\": \"object\",\n      \"description\": \"A custom downloader definition that enables the plugin to handle a custom URL scheme when Helm resolves chart repositories.\",\n      \"required\": [\n        \"command\",\n        \"protocols\"\n      ],\n      \"properties\": {\n        \"command\": {\n          \"type\": \"string\",\n          \"description\": \"The command to run for downloading. Receives the URI as the final argument.\"\n        },\n        \"protocols\": {\n          \"type\": \"array\",\n          \"description\": \"List of URI scheme prefixes this downloader handles.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"examples\": [\n            [\"s3://\"],\n            [\"gs://\"],\n            [\"oci://\"]\n          ]\n        }\n      }\n    },\n    \"PlatformCommand\": {\n      \"type\": \"object\",\n      \"description\": \"A platform-specific command override. Helm\
  \ matches the current OS and architecture against all entries and uses the first match.\",\n      \"required\": [\n        \"command\"\n      ],\n      \"properties\": {\n        \"os\": {\n          \"type\": \"string\",\n          \"description\": \"The operating system this entry applies to. Matches GOOS values.\",\n          \"enum\": [\n            \"linux\",\n            \"darwin\",\n            \"windows\",\n            \"freebsd\"\n          ]\n        },\n        \"arch\": {\n          \"type\": \"string\",\n          \"description\": \"The CPU architecture this entry applies to. Matches GOARCH values.\",\n          \"enum\": [\n            \"amd64\",\n            \"arm64\",\n            \"arm\",\n            \"386\",\n            \"s390x\",\n            \"ppc64le\"\n          ]\n        },\n        \"command\": {\n          \"type\": \"string\",\n          \"description\": \"The command to run on this platform. Overrides the top-level command field.\",\n          \"examples\"\
  : [\n            \"$HELM_PLUGIN_DIR/bin/helm-diff-linux-amd64\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/helm/refs/heads/main/json-schema/helm-plugin-schema.json
tags:
- Charts
- Cloud Native
- Container Orchestration
- DevOps
- Kubernetes
- Package Manager
title: Helm Plugin Descriptor
---
