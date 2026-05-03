---
description: A Webflow Site object representing a website within a workspace, as returned by the GET /sites/{site_id} endpoint of the Webflow Data API v2.
layout: schema
name: Webflow Site
properties_list:
- description: Unique identifier for the Site.
  name: id
  type: string
- description: Unique identifier for the Workspace that contains this Site.
  name: workspaceId
  type: string
- description: Name given to the Site.
  name: displayName
  type: string
- description: Slugified version of the Site name.
  name: shortName
  type: string
- description: URL of a generated screenshot image for the given Site.
  name: previewUrl
  type: string
- description: Site timezone set under Site Settings.
  name: timeZone
  type: string
- description: Date the Site was created.
  name: createdOn
  type: string
- description: Date the Site was last updated.
  name: lastUpdated
  type: string
- description: Date the Site was last published.
  name: lastPublished
  type: string
- description: The ID of the parent folder the Site exists in.
  name: parentFolderId
  type:
  - string
  - 'null'
- description: A list of custom domains registered to this Site.
  name: customDomains
  type: array
- description: Locale configuration for the Site, including primary and secondary locales.
  name: locales
  type: object
- description: Indicates if data collection is enabled for the site.
  name: dataCollectionEnabled
  type: boolean
- description: The type of data collection enabled for the site.
  name: dataCollectionType
  type: string
provider_name: Webflow
provider_slug: webflow
schema_file: json-schema/webflow-site-schema.json
slug: webflow-site
source_filename: webflow-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.webflow.com/schemas/site.json\",\n  \"title\": \"Webflow Site\",\n  \"description\": \"A Webflow Site object representing a website within a workspace, as returned by the GET /sites/{site_id} endpoint of the Webflow Data API v2.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the Site.\",\n      \"examples\": [\"580e63e98c9a982ac9b8b741\"]\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the Workspace that contains this Site.\",\n      \"examples\": [\"580e63e98c9a982ac9b8b741\"]\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Name given to the Site.\",\n      \"examples\": [\"api_docs_sample_json\"]\n    },\n    \"shortName\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Slugified version of the Site name.\",\n      \"examples\": [\"api-docs-sample-json\"]\n    },\n    \"previewUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of a generated screenshot image for the given Site.\",\n      \"examples\": [\"https://screenshots.webflow.com/sites/6258612d1ee792848f805dcf/20231219211811_d5990556c743f33b7071300a03bf67e6.png\"]\n    },\n    \"timeZone\": {\n      \"type\": \"string\",\n      \"description\": \"Site timezone set under Site Settings.\",\n      \"examples\": [\"America/Los_Angeles\"]\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the Site was created.\",\n      \"examples\": [\"2016-10-24T19:41:29.156Z\"]\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the Site was last updated.\",\n      \"examples\": [\"2016-10-24T19:43:17.271Z\"\
  ]\n    },\n    \"lastPublished\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the Site was last published.\",\n      \"examples\": [\"2016-10-24T19:43:17.271Z\"]\n    },\n    \"parentFolderId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the parent folder the Site exists in.\",\n      \"examples\": [\"1as2d3f4g5h6j7k8l9z0x1c2v3b4n5m6\"]\n    },\n    \"customDomains\": {\n      \"type\": \"array\",\n      \"description\": \"A list of custom domains registered to this Site.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"id\"],\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the Domain.\",\n            \"examples\": [\"589a331aa51e760df7ccb89d\"]\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"description\": \"The registered Domain name.\",\n  \
  \          \"examples\": [\"test-api-domain.com\"]\n          },\n          \"lastPublished\": {\n            \"type\": [\"string\", \"null\"],\n            \"format\": \"date-time\",\n            \"description\": \"The date the custom domain was last published to.\",\n            \"readOnly\": true,\n            \"examples\": [\"2022-12-07T16:51:37.571Z\"]\n          }\n        }\n      }\n    },\n    \"locales\": {\n      \"type\": \"object\",\n      \"description\": \"Locale configuration for the Site, including primary and secondary locales.\",\n      \"properties\": {\n        \"primary\": {\n          \"type\": \"object\",\n          \"description\": \"The primary locale for the site.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The unique identifier for the locale.\",\n              \"examples\": [\"653fd9af6a07fc9cfd7a5e57\"]\n            },\n            \"cmsLocaleId\": {\n              \"type\":\
  \ \"string\",\n              \"description\": \"A CMS-specific identifier for the locale.\",\n              \"examples\": [\"653ad57de882f528b32e810e\"]\n            },\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"description\": \"Indicates if the locale is enabled.\",\n              \"examples\": [false]\n            },\n            \"displayName\": {\n              \"type\": \"string\",\n              \"description\": \"The display name of the locale, typically in English.\",\n              \"examples\": [\"English (United States)\"]\n            },\n            \"displayImageId\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"An optional ID for an image associated with the locale.\",\n              \"examples\": [null]\n            },\n            \"redirect\": {\n              \"type\": \"boolean\",\n              \"description\": \"Determines if requests should redirect to the locale's subdirectory.\",\n\
  \              \"examples\": [true]\n            },\n            \"subdirectory\": {\n              \"type\": \"string\",\n              \"description\": \"The subdirectory path for the locale, used in URLs.\",\n              \"examples\": [\"\"]\n            },\n            \"tag\": {\n              \"type\": \"string\",\n              \"description\": \"A tag or code representing the locale, following a standard format like 'en-US'.\",\n              \"examples\": [\"en-US\"]\n            }\n          }\n        },\n        \"secondary\": {\n          \"type\": \"array\",\n          \"description\": \"A list of secondary locales available for the site.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"The unique identifier for the locale.\",\n                \"examples\": [\"653fd9af6a07fc9cfd7a5e56\"]\n              },\n              \"cmsLocaleId\"\
  : {\n                \"type\": \"string\",\n                \"description\": \"A CMS-specific identifier for the locale.\",\n                \"examples\": [\"653fd9af6a07fc9cfd7a5e5d\"]\n              },\n              \"enabled\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates if the locale is enabled.\",\n                \"examples\": [true]\n              },\n              \"displayName\": {\n                \"type\": \"string\",\n                \"description\": \"The display name of the locale, typically in English.\",\n                \"examples\": [\"French (France)\"]\n              },\n              \"displayImageId\": {\n                \"type\": [\"string\", \"null\"],\n                \"description\": \"An optional ID for an image associated with the locale.\",\n                \"examples\": [null]\n              },\n              \"subdirectory\": {\n                \"type\": \"string\",\n                \"description\": \"The subdirectory\
  \ path for the locale, used in URLs.\",\n                \"examples\": [\"fr-fr\"]\n              },\n              \"tag\": {\n                \"type\": \"string\",\n                \"description\": \"A tag or code representing the locale, following a standard format like 'en-US'.\",\n                \"examples\": [\"fr-FR\"]\n              }\n            }\n          }\n        }\n      }\n    },\n    \"dataCollectionEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if data collection is enabled for the site.\",\n      \"examples\": [false]\n    },\n    \"dataCollectionType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of data collection enabled for the site.\",\n      \"enum\": [\n        \"always\",\n        \"optOut\",\n        \"disabled\"\n      ],\n      \"examples\": [\"always\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/json-schema/webflow-site-schema.json
tags:
- CMS
- Ecommerce
- No-Code
- Web Development
title: Webflow Site
---
