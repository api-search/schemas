---
description: A project in Dataiku DSS that serves as the top-level organizational unit containing datasets, recipes, models, scenarios, and other data science artifacts.
layout: schema
name: Dataiku DSS Project
properties_list:
- description: Unique project key identifier, typically uppercase letters and numbers
  name: projectKey
  type: string
- description: Display name of the project
  name: name
  type: string
- description: Login of the project owner
  name: owner
  type: string
- description: Detailed description of the project
  name: description
  type: string
- description: Short one-line description of the project
  name: shortDesc
  type: string
- description: Current lifecycle status of the project
  name: projectStatus
  type: string
- description: Tags associated with the project for categorization
  name: tags
  type: array
- description: Project checklists for tracking tasks and milestones
  name: checklists
  type: object
- description: Access permissions for the project
  name: permissions
  type: array
- description: ''
  name: creationTag
  type: object
- description: ''
  name: versionTag
  type: object
- description: ''
  name: settings
  type: object
provider_name: Dataiku
provider_slug: dataiku
schema_file: json-schema/dataiku-project-schema.json
slug: dataiku-project
source_filename: dataiku-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://doc.dataiku.com/schemas/dataiku/project.json\",\n  \"title\": \"Dataiku DSS Project\",\n  \"description\": \"A project in Dataiku DSS that serves as the top-level organizational unit containing datasets, recipes, models, scenarios, and other data science artifacts.\",\n  \"type\": \"object\",\n  \"required\": [\"projectKey\", \"name\"],\n  \"properties\": {\n    \"projectKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique project key identifier, typically uppercase letters and numbers\",\n      \"pattern\": \"^[A-Z][A-Z0-9_]*$\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the project\",\n      \"minLength\": 1\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Login of the project owner\"\n    },\n    \"description\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Detailed description of the project\"\n    },\n    \"shortDesc\": {\n      \"type\": \"string\",\n      \"description\": \"Short one-line description of the project\"\n    },\n    \"projectStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"Sandbox\", \"In Design\", \"In Production\", \"Archived\"],\n      \"description\": \"Current lifecycle status of the project\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags associated with the project for categorization\"\n    },\n    \"checklists\": {\n      \"type\": \"object\",\n      \"description\": \"Project checklists for tracking tasks and milestones\",\n      \"properties\": {\n        \"checklists\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Checklist\"\n          }\n        }\n      }\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n\
  \      \"items\": {\n        \"$ref\": \"#/$defs/Permission\"\n      },\n      \"description\": \"Access permissions for the project\"\n    },\n    \"creationTag\": {\n      \"$ref\": \"#/$defs/VersionTag\"\n    },\n    \"versionTag\": {\n      \"$ref\": \"#/$defs/VersionTag\"\n    },\n    \"settings\": {\n      \"$ref\": \"#/$defs/ProjectSettings\"\n    }\n  },\n  \"$defs\": {\n    \"VersionTag\": {\n      \"type\": \"object\",\n      \"description\": \"Version tracking information\",\n      \"properties\": {\n        \"versionNumber\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Sequential version number\"\n        },\n        \"lastModifiedBy\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"login\": {\n              \"type\": \"string\",\n              \"description\": \"Login of the user who made the modification\"\n            }\n          }\n        },\n        \"lastModifiedOn\": {\n          \"type\"\
  : \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the last modification\"\n        }\n      }\n    },\n    \"Permission\": {\n      \"type\": \"object\",\n      \"description\": \"A permission entry granting access to a user or group\",\n      \"properties\": {\n        \"group\": {\n          \"type\": \"string\",\n          \"description\": \"Group name to grant permissions to\"\n        },\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"User login to grant permissions to\"\n        },\n        \"readProjectContent\": {\n          \"type\": \"boolean\",\n          \"description\": \"Can read project content\"\n        },\n        \"writeProjectContent\": {\n          \"type\": \"boolean\",\n          \"description\": \"Can write project content\"\n        },\n        \"admin\": {\n          \"type\": \"boolean\",\n          \"description\": \"Has admin permissions on the project\"\n        },\n        \"\
  readDashboards\": {\n          \"type\": \"boolean\",\n          \"description\": \"Can read dashboards\"\n        },\n        \"writeDashboards\": {\n          \"type\": \"boolean\",\n          \"description\": \"Can write dashboards\"\n        },\n        \"runScenarios\": {\n          \"type\": \"boolean\",\n          \"description\": \"Can run scenarios\"\n        },\n        \"manageDashboardAuthorizations\": {\n          \"type\": \"boolean\",\n          \"description\": \"Can manage dashboard authorizations\"\n        },\n        \"executeApp\": {\n          \"type\": \"boolean\",\n          \"description\": \"Can execute project as an application\"\n        }\n      }\n    },\n    \"Checklist\": {\n      \"type\": \"object\",\n      \"description\": \"A checklist with title and items\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Checklist title\"\n        },\n        \"items\": {\n          \"type\": \"array\",\n\
  \          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"done\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether the item is completed\"\n              },\n              \"text\": {\n                \"type\": \"string\",\n                \"description\": \"Item description\"\n              },\n              \"createdBy\": {\n                \"type\": \"string\",\n                \"description\": \"User who created the item\"\n              },\n              \"createdOn\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"ProjectSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Project-level settings\",\n      \"properties\": {\n        \"flowBuildSettings\": {\n          \"type\": \"object\",\n          \"description\": \"Default build settings for the project flow\",\n\
  \          \"properties\": {\n            \"mergeSparkPipelines\": {\n              \"type\": \"boolean\"\n            },\n            \"pruneBeforeSparkPipelines\": {\n              \"type\": \"boolean\"\n            }\n          }\n        },\n        \"codeEnvs\": {\n          \"type\": \"object\",\n          \"description\": \"Code environment settings\",\n          \"properties\": {\n            \"python\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"mode\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"INHERIT\", \"EXPLICIT_ENV\", \"CUSTOM\"],\n                  \"description\": \"Python environment selection mode\"\n                },\n                \"envName\": {\n                  \"type\": \"string\",\n                  \"description\": \"Name of the code environment\"\n                }\n              }\n            },\n            \"r\": {\n              \"type\": \"object\",\n              \"properties\"\
  : {\n                \"mode\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"INHERIT\", \"EXPLICIT_ENV\", \"CUSTOM\"],\n                  \"description\": \"R environment selection mode\"\n                },\n                \"envName\": {\n                  \"type\": \"string\",\n                  \"description\": \"Name of the code environment\"\n                }\n              }\n            }\n          }\n        },\n        \"integrations\": {\n          \"type\": \"object\",\n          \"description\": \"Integration settings (Git, etc.)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dataiku/refs/heads/main/json-schema/dataiku-project-schema.json
tags:
- Analytics
- Artificial Intelligence
- Data Platform
- Data Science
- Machine Learning
title: Dataiku DSS Project
---
