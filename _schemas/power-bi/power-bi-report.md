---
description: Schema for a Power BI report resource as returned by the Power BI REST API. A report is a multi-page visual presentation of data from a dataset, with interactive elements for filtering, drilling, and exploring insights.
layout: schema
name: Power BI Report
properties_list:
- description: The unique identifier of the report, assigned by the Power BI service
  name: id
  type: string
- description: The display name of the report
  name: name
  type: string
- description: A text description of the report's purpose and content
  name: description
  type: string
- description: The unique identifier of the dataset that provides data to this report
  name: datasetId
  type: string
- description: The type of report, either an interactive Power BI report or a paginated report
  name: reportType
  type: string
- description: The web URL for viewing the report in the Power BI service
  name: webUrl
  type: string
- description: The URL for embedding the report in third-party applications using the Power BI Embedded service
  name: embedUrl
  type: string
- description: The UTC date and time when the report was first created
  name: createdDateTime
  type: string
- description: The UTC date and time when the report was last modified
  name: modifiedDateTime
  type: string
- description: The display name or email of the user who last modified the report
  name: modifiedBy
  type: string
- description: The display name or email of the user who created the report
  name: createdBy
  type: string
- description: The unique identifier of the workspace containing this report
  name: workspaceId
  type: string
- description: The pages within the report, each containing visualizations and layout
  name: pages
  type: array
- description: The workspace ID of the dataset if it resides in a different workspace from the report
  name: datasetWorkspaceId
  type: string
- description: The app ID if this report is part of a published Power BI app
  name: appId
  type: string
- description: Users who have access to the report and their permissions
  name: users
  type: array
- description: Email subscriptions configured for this report
  name: subscriptions
  type: array
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-report-schema.json
slug: power-bi-report
source_filename: power-bi-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/schemas/power-bi/report.json\",\n  \"title\": \"Power BI Report\",\n  \"description\": \"Schema for a Power BI report resource as returned by the Power BI REST API. A report is a multi-page visual presentation of data from a dataset, with interactive elements for filtering, drilling, and exploring insights.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the report, assigned by the Power BI service\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the report\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A text description of the report's purpose and content\"\n    },\n \
  \   \"datasetId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the dataset that provides data to this report\"\n    },\n    \"reportType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of report, either an interactive Power BI report or a paginated report\",\n      \"enum\": [\"PowerBIReport\", \"PaginatedReport\"]\n    },\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The web URL for viewing the report in the Power BI service\"\n    },\n    \"embedUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for embedding the report in third-party applications using the Power BI Embedded service\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The UTC date and time when the report was first created\"\n    },\n    \"modifiedDateTime\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The UTC date and time when the report was last modified\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The display name or email of the user who last modified the report\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The display name or email of the user who created the report\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the workspace containing this report\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"The pages within the report, each containing visualizations and layout\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Page\"\n      }\n    },\n    \"datasetWorkspaceId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The workspace ID of the\
  \ dataset if it resides in a different workspace from the report\"\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The app ID if this report is part of a published Power BI app\"\n    },\n    \"users\": {\n      \"type\": \"array\",\n      \"description\": \"Users who have access to the report and their permissions\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ReportUser\"\n      }\n    },\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"description\": \"Email subscriptions configured for this report\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Subscription\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Page\": {\n      \"type\": \"object\",\n      \"description\": \"A page within a Power BI report containing visualizations and layout\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The internal name of the page, used as a unique identifier\
  \ within the report\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name shown in the report page tab\"\n        },\n        \"order\": {\n          \"type\": \"integer\",\n          \"description\": \"The zero-based order of the page within the report\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"ReportUser\": {\n      \"type\": \"object\",\n      \"description\": \"A user with access to the report\",\n      \"properties\": {\n        \"emailAddress\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the user\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user\"\n        },\n        \"identifier\": {\n          \"type\": \"string\",\n          \"description\": \"The object ID of the user in Azure Active Directory\"\n        },\n        \"reportUserAccessRight\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The access right the user has on the report\",\n          \"enum\": [\"Owner\", \"ReadWrite\", \"Read\", \"ReadReshare\", \"ReadCopy\", \"ReadReshareExplore\"]\n        },\n        \"principalType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of principal\",\n          \"enum\": [\"User\", \"Group\", \"App\"]\n        }\n      }\n    },\n    \"Subscription\": {\n      \"type\": \"object\",\n      \"description\": \"An email subscription for a report or report page\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the subscription\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The subject line of the subscription email\"\n        },\n        \"artifactId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\
  ,\n          \"description\": \"The report ID this subscription is for\"\n        },\n        \"artifactDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the report\"\n        },\n        \"subArtifactDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the specific report page if applicable\"\n        },\n        \"frequency\": {\n          \"type\": \"string\",\n          \"description\": \"How often the subscription email is sent\",\n          \"enum\": [\"Daily\", \"Weekly\", \"Monthly\"]\n        },\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The start date and time for the subscription\"\n        },\n        \"endDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The end date and time for the subscription\"\n        },\n        \"isEnabled\": {\n\
  \          \"type\": \"boolean\",\n          \"description\": \"Whether the subscription is currently active\"\n        },\n        \"users\": {\n          \"type\": \"array\",\n          \"description\": \"The recipients of the subscription email\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"emailAddress\": {\n                \"type\": \"string\",\n                \"format\": \"email\"\n              },\n              \"displayName\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-report-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Power BI Report
---
