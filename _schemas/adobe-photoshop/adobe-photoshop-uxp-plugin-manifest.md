---
description: Schema for the manifest.json file required by UXP plugins for Adobe Photoshop. The manifest defines plugin metadata, entry points, permissions, and host application requirements.
layout: schema
name: Adobe Photoshop UXP Plugin Manifest
properties_list:
- description: Unique plugin identifier. Use reverse domain notation (e.g., com.example.myplugin).
  name: id
  type: string
- description: Display name of the plugin shown in the Photoshop UI.
  name: name
  type: string
- description: Plugin version in semver format (major.minor.patch).
  name: version
  type: string
- description: UXP manifest schema version. Version 5 or 6 recommended for current Photoshop.
  name: manifestVersion
  type: integer
- description: Path to the main JavaScript entry point file relative to the plugin root.
  name: main
  type: string
- description: Host application requirements.
  name: host
  type: object
- description: Plugin entry points defining panels, commands, and other UI elements.
  name: entrypoints
  type: array
- description: Plugin icons at various sizes for different display contexts.
  name: icons
  type: array
- description: Permissions the plugin requires to function.
  name: requiredPermissions
  type: object
- description: Configuration for hybrid plugin native C++ addon.
  name: addon
  type: object
- description: Short description of the plugin's purpose.
  name: description
  type: string
- description: Plugin author or company name.
  name: author
  type: string
- description: Keywords for plugin discovery in the Adobe Marketplace.
  name: keywords
  type: array
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-uxp-plugin-manifest-schema.json
slug: adobe-photoshop-uxp-plugin-manifest
source_filename: adobe-photoshop-uxp-plugin-manifest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.adobe.com/photoshop/uxp/plugin-manifest.schema.json\",\n  \"title\": \"Adobe Photoshop UXP Plugin Manifest\",\n  \"description\": \"Schema for the manifest.json file required by UXP plugins for Adobe Photoshop. The manifest defines plugin metadata, entry points, permissions, and host application requirements.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"version\",\n    \"manifestVersion\",\n    \"host\",\n    \"entrypoints\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique plugin identifier. Use reverse domain notation (e.g., com.example.myplugin).\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the plugin shown in the Photoshop UI.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\
  \\d+$\",\n      \"description\": \"Plugin version in semver format (major.minor.patch).\"\n    },\n    \"manifestVersion\": {\n      \"type\": \"integer\",\n      \"enum\": [4, 5, 6],\n      \"description\": \"UXP manifest schema version. Version 5 or 6 recommended for current Photoshop.\"\n    },\n    \"main\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the main JavaScript entry point file relative to the plugin root.\"\n    },\n    \"host\": {\n      \"type\": \"object\",\n      \"description\": \"Host application requirements.\",\n      \"required\": [\n        \"app\",\n        \"minVersion\"\n      ],\n      \"properties\": {\n        \"app\": {\n          \"type\": \"string\",\n          \"const\": \"PS\",\n          \"description\": \"Host application identifier. PS for Adobe Photoshop.\"\n        },\n        \"minVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum required Photoshop version (e.g., 22.0.0 for UXP support).\"\n\
  \        },\n        \"maxVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Optional maximum supported Photoshop version.\"\n        }\n      }\n    },\n    \"entrypoints\": {\n      \"type\": \"array\",\n      \"description\": \"Plugin entry points defining panels, commands, and other UI elements.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"type\",\n          \"id\",\n          \"label\"\n        ],\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"panel\",\n              \"command\"\n            ],\n            \"description\": \"Entry point type. panel creates a dockable panel, command creates a menu item.\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for this entry point within the plugin.\"\n          },\n          \"label\": {\n            \"type\": \"object\"\
  ,\n            \"description\": \"Localized display labels for the entry point.\",\n            \"properties\": {\n              \"default\": {\n                \"type\": \"string\",\n                \"description\": \"Default display label.\"\n              }\n            },\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            }\n          },\n          \"minimumSize\": {\n            \"type\": \"object\",\n            \"description\": \"Minimum panel dimensions (panel type only).\",\n            \"properties\": {\n              \"width\": {\n                \"type\": \"integer\"\n              },\n              \"height\": {\n                \"type\": \"integer\"\n              }\n            }\n          },\n          \"maximumSize\": {\n            \"type\": \"object\",\n            \"description\": \"Maximum panel dimensions (panel type only).\",\n            \"properties\": {\n              \"width\": {\n                \"type\": \"integer\"\n\
  \              },\n              \"height\": {\n                \"type\": \"integer\"\n              }\n            }\n          },\n          \"preferredDockedSize\": {\n            \"type\": \"object\",\n            \"description\": \"Preferred panel dimensions when docked.\",\n            \"properties\": {\n              \"width\": {\n                \"type\": \"integer\"\n              },\n              \"height\": {\n                \"type\": \"integer\"\n              }\n            }\n          },\n          \"preferredFloatingSize\": {\n            \"type\": \"object\",\n            \"description\": \"Preferred panel dimensions when floating.\",\n            \"properties\": {\n              \"width\": {\n                \"type\": \"integer\"\n              },\n              \"height\": {\n                \"type\": \"integer\"\n              }\n            }\n          },\n          \"shortcut\": {\n            \"type\": \"object\",\n            \"description\": \"Keyboard shortcut\
  \ for the entry point.\",\n            \"properties\": {\n              \"mac\": {\n                \"type\": \"string\",\n                \"description\": \"macOS keyboard shortcut.\"\n              },\n              \"win\": {\n                \"type\": \"string\",\n                \"description\": \"Windows keyboard shortcut.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"icons\": {\n      \"type\": \"array\",\n      \"description\": \"Plugin icons at various sizes for different display contexts.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"width\",\n          \"height\",\n          \"path\"\n        ],\n        \"properties\": {\n          \"width\": {\n            \"type\": \"integer\",\n            \"description\": \"Icon width in pixels.\"\n          },\n          \"height\": {\n            \"type\": \"integer\",\n            \"description\": \"Icon height in pixels.\"\n          },\n          \"path\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"Path to the icon file relative to the plugin root.\"\n          },\n          \"scale\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"number\"\n            },\n            \"description\": \"Display scale factors (e.g., [1, 2] for standard and Retina).\"\n          },\n          \"theme\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"lightest\",\n                \"light\",\n                \"medium\",\n                \"dark\",\n                \"darkest\",\n                \"all\"\n              ]\n            },\n            \"description\": \"UI themes this icon supports.\"\n          }\n        }\n      }\n    },\n    \"requiredPermissions\": {\n      \"type\": \"object\",\n      \"description\": \"Permissions the plugin requires to function.\",\n      \"properties\": {\n\
  \        \"clipboard\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"read\",\n            \"readAndWrite\"\n          ],\n          \"description\": \"Clipboard access level.\"\n        },\n        \"network\": {\n          \"type\": \"object\",\n          \"description\": \"Network access permissions.\",\n          \"properties\": {\n            \"domains\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Allowed network domains. Use 'all' for unrestricted access.\"\n            }\n          }\n        },\n        \"webview\": {\n          \"type\": \"object\",\n          \"description\": \"WebView permissions for embedded web content.\",\n          \"properties\": {\n            \"allow\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"yes\",\n                \"no\"\n              ]\n            },\n            \"\
  domains\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"ipc\": {\n          \"type\": \"object\",\n          \"description\": \"Inter-plugin communication permissions.\",\n          \"properties\": {\n            \"enablePluginCommunication\": {\n              \"type\": \"boolean\"\n            }\n          }\n        },\n        \"allowCodeGenerationFromStrings\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to allow eval() and Function() from strings.\"\n        },\n        \"localFileSystem\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"plugin\",\n            \"request\",\n            \"fullAccess\"\n          ],\n          \"description\": \"File system access level. plugin = plugin sandbox only, request = user-prompted, fullAccess = unrestricted.\"\n        },\n        \"launchProcess\": {\n       \
  \   \"type\": \"object\",\n          \"description\": \"Permission to launch external processes (hybrid plugins).\",\n          \"properties\": {\n            \"schemes\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"extensions\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"enableAddon\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to enable native C++ addon loading (hybrid plugins).\"\n        }\n      }\n    },\n    \"addon\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for hybrid plugin native C++ addon.\",\n      \"properties\": {\n        \"cplugins\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\"\
  : {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"filter\"\n                ]\n              },\n              \"path\": {\n                \"type\": \"string\",\n                \"description\": \"Relative path to the .uxpaddon file.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the plugin's purpose.\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Plugin author or company name.\"\n    },\n    \"keywords\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Keywords for plugin discovery in the Adobe Marketplace.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-uxp-plugin-manifest-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: Adobe Photoshop UXP Plugin Manifest
---
