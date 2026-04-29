---
description: A Tableau workbook containing one or more views (worksheets, dashboards, or stories) that connect to data sources and provide interactive visual analytics.
layout: schema
name: Tableau Workbook
properties_list:
- description: The unique identifier (LUID) for the workbook.
  name: id
  type: string
- description: The name of the workbook as it appears on the server.
  name: name
  type: string
- description: A user-provided description of the workbook.
  name: description
  type:
  - string
  - 'null'
- description: The URL-friendly name of the workbook used in the content URL path. Automatically generated from the workbook name.
  name: contentUrl
  type: string
- description: The full URL to view the workbook in a web browser on Tableau Server or Tableau Cloud.
  name: webpageUrl
  type: string
- description: Whether the workbook displays views as navigable tabs.
  name: showTabs
  type: boolean
- description: The size of the workbook file in bytes.
  name: size
  type: integer
- description: The ISO 8601 timestamp when the workbook was first published to the server.
  name: createdAt
  type: string
- description: The ISO 8601 timestamp when the workbook was last modified or republished.
  name: updatedAt
  type: string
- description: Whether extracts embedded in the workbook are encrypted at rest.
  name: encryptExtracts
  type: string
- description: The ID of the view that is displayed by default when the workbook is opened.
  name: defaultViewId
  type:
  - string
  - 'null'
- description: ''
  name: project
  type: object
- description: ''
  name: owner
  type: object
- description: Tags associated with the workbook for categorization and search.
  name: tags
  type: object
- description: The views (worksheets, dashboards, and stories) contained in the workbook.
  name: views
  type: object
- description: The data connections used by the workbook.
  name: connections
  type: object
- description: ''
  name: usage
  type: object
- description: Configuration for Data Acceleration on the workbook.
  name: dataAccelerationConfig
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-workbook-schema.json
slug: tableau-workbook
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://help.tableau.com/schemas/tableau/workbook.json\",\n  \"title\": \"Tableau Workbook\",\n  \"description\": \"A Tableau workbook containing one or more views (worksheets, dashboards, or stories) that connect to data sources and provide interactive visual analytics.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier (LUID) for the workbook.\",\n      \"pattern\": \"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workbook as it appears on the server.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A user-provided description of the workbook.\"\
  ,\n      \"maxLength\": 4000\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly name of the workbook used in the content URL path. Automatically generated from the workbook name.\"\n    },\n    \"webpageUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The full URL to view the workbook in a web browser on Tableau Server or Tableau Cloud.\"\n    },\n    \"showTabs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workbook displays views as navigable tabs.\",\n      \"default\": false\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The size of the workbook file in bytes.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the workbook was first published to the server.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the workbook was last modified or republished.\"\n    },\n    \"encryptExtracts\": {\n      \"type\": \"string\",\n      \"description\": \"Whether extracts embedded in the workbook are encrypted at rest.\"\n    },\n    \"defaultViewId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the view that is displayed by default when the workbook is opened.\",\n      \"pattern\": \"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$\"\n    },\n    \"project\": {\n      \"$ref\": \"#/$defs/ProjectReference\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/$defs/OwnerReference\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags associated with the workbook for categorization and search.\",\n      \"properties\": {\n        \"tag\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Tag\"\
  \n          }\n        }\n      }\n    },\n    \"views\": {\n      \"type\": \"object\",\n      \"description\": \"The views (worksheets, dashboards, and stories) contained in the workbook.\",\n      \"properties\": {\n        \"view\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/View\"\n          }\n        }\n      }\n    },\n    \"connections\": {\n      \"type\": \"object\",\n      \"description\": \"The data connections used by the workbook.\",\n      \"properties\": {\n        \"connection\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Connection\"\n          }\n        }\n      }\n    },\n    \"usage\": {\n      \"$ref\": \"#/$defs/Usage\"\n    },\n    \"dataAccelerationConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for Data Acceleration on the workbook.\",\n      \"properties\": {\n        \"accelerationEnabled\": {\n          \"type\": \"boolean\",\n\
  \          \"description\": \"Whether Data Acceleration is enabled.\"\n        },\n        \"accelerateNow\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to accelerate immediately.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"ProjectReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to the project that contains the workbook.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the project.\",\n          \"pattern\": \"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the project.\"\n        }\n      }\n    },\n    \"OwnerReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to the user who owns the workbook.\",\n      \"required\": [\"id\"\
  ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the owner.\",\n          \"pattern\": \"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the owner.\"\n        }\n      }\n    },\n    \"View\": {\n      \"type\": \"object\",\n      \"description\": \"A view (worksheet, dashboard, or story) within a workbook.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the view.\",\n          \"pattern\": \"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the view.\"\n        },\n        \"contentUrl\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The URL-friendly name used in the content URL.\"\n        },\n        \"viewUrlName\": {\n          \"type\": \"string\",\n          \"description\": \"The URL-safe name of the view.\"\n        },\n        \"sheetType\": {\n          \"type\": \"string\",\n          \"enum\": [\"worksheet\", \"dashboard\", \"story\"],\n          \"description\": \"The type of sheet: worksheet, dashboard, or story.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the view was created.\"\n        },\n        \"updatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the view was last updated.\"\n        },\n        \"tags\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"tag\": {\n              \"type\": \"array\",\n              \"items\": {\n        \
  \        \"$ref\": \"#/$defs/Tag\"\n              }\n            }\n          }\n        },\n        \"usage\": {\n          \"$ref\": \"#/$defs/Usage\"\n        }\n      }\n    },\n    \"Connection\": {\n      \"type\": \"object\",\n      \"description\": \"A data connection within a workbook, representing a link to a data source.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the connection.\",\n          \"pattern\": \"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of data connection (e.g., sqlserver, postgres, mysql, oracle, snowflake, bigquery, redshift, excel, hyper, textscan, googlesheets).\"\n        },\n        \"serverAddress\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The hostname or IP address of the database server.\"\
  \n        },\n        \"serverPort\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The port number used for the connection.\"\n        },\n        \"userName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The user name used to authenticate with the data source.\"\n        },\n        \"datasource\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to the published data source, if applicable.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The ID of the published data source.\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The name of the published data source.\"\n            }\n          }\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A tag label applied to content for organization and discoverability.\"\
  ,\n      \"required\": [\"label\"],\n      \"properties\": {\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"The text of the tag.\",\n          \"minLength\": 1,\n          \"maxLength\": 255\n        }\n      }\n    },\n    \"Usage\": {\n      \"type\": \"object\",\n      \"description\": \"Usage statistics for the content.\",\n      \"properties\": {\n        \"totalViewCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The total number of times the content has been viewed.\"\n        }\n      }\n    },\n    \"Revision\": {\n      \"type\": \"object\",\n      \"description\": \"A published revision of the workbook.\",\n      \"properties\": {\n        \"revisionNumber\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The sequential revision number.\"\n        },\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\
  ,\n          \"description\": \"When this revision was published.\"\n        },\n        \"deleted\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this revision has been deleted.\"\n        },\n        \"current\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the current (latest) revision.\"\n        },\n        \"sizeInBytes\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The size of this revision in bytes.\"\n        },\n        \"publisher\": {\n          \"$ref\": \"#/$defs/OwnerReference\"\n        }\n      }\n    },\n    \"Permission\": {\n      \"type\": \"object\",\n      \"description\": \"A permission rule granting or denying capabilities to a user or group.\",\n      \"properties\": {\n        \"granteeCapabilities\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"user\"\
  : {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"description\": \"The ID of the user grantee.\"\n                  }\n                }\n              },\n              \"group\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"description\": \"The ID of the group grantee.\"\n                  }\n                }\n              },\n              \"capabilities\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"capability\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\": \"object\",\n                      \"properties\": {\n                        \"name\": {\n                          \"type\": \"string\",\n                       \
  \   \"enum\": [\n                            \"Read\",\n                            \"Write\",\n                            \"Filter\",\n                            \"AddComment\",\n                            \"ViewComments\",\n                            \"ShareView\",\n                            \"ExportData\",\n                            \"ExportImage\",\n                            \"ExportXml\",\n                            \"Delete\",\n                            \"ChangePermissions\",\n                            \"ViewUnderlyingData\",\n                            \"WebAuthoring\",\n                            \"RunExplainData\",\n                            \"CreateRefreshMetrics\",\n                            \"ChangeHierarchy\"\n                          ],\n                          \"description\": \"The name of the capability.\"\n                        },\n                        \"mode\": {\n                          \"type\": \"string\",\n                         \
  \ \"enum\": [\"Allow\", \"Deny\"],\n                          \"description\": \"Whether the capability is allowed or denied.\"\n                        }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-workbook-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Tableau Workbook
---
