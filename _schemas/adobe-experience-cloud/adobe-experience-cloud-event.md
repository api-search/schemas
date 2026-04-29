---
description: An experience event representing a time-series observation of an action or state change associated with a profile, such as a page view, product interaction, purchase, or campaign engagement.
layout: schema
name: Adobe Experience Cloud Event
properties_list:
- description: A unique identifier for this event instance.
  name: eventId
  type: string
- description: The type of experience event.
  name: eventType
  type: string
- description: The ISO 8601 timestamp when the event occurred.
  name: timestamp
  type: string
- description: Identity namespaces and values associated with this event.
  name: identityMap
  type: object
- description: Web-specific event details.
  name: web
  type: object
- description: Commerce-specific event details.
  name: commerce
  type: object
- description: The device used during the event.
  name: device
  type: object
- description: Environment details at the time of the event.
  name: environment
  type: object
- description: The source system that generated the event.
  name: source
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/adobe-experience-cloud-event.json
slug: adobe-experience-cloud-event
source_filename: adobe-experience-cloud-event.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"adobe-experience-cloud-event.json\",\n  \"title\": \"Adobe Experience Cloud Event\",\n  \"description\": \"An experience event representing a time-series observation of an action or state change associated with a profile, such as a page view, product interaction, purchase, or campaign engagement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this event instance.\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of experience event.\",\n      \"enum\": [\n        \"web.webpagedetails.pageViews\",\n        \"web.webinteraction.linkClicks\",\n        \"commerce.productViews\",\n        \"commerce.productListAdds\",\n        \"commerce.purchases\",\n        \"commerce.checkouts\",\n        \"campaign.sent\",\n        \"campaign.opened\",\n        \"campaign.clicked\"\
  ,\n        \"campaign.bounced\",\n        \"pushTracking.applicationOpened\",\n        \"pushTracking.customAction\",\n        \"decisioning.propositionDisplay\",\n        \"decisioning.propositionInteract\"\n      ]\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the event occurred.\"\n    },\n    \"identityMap\": {\n      \"type\": \"object\",\n      \"description\": \"Identity namespaces and values associated with this event.\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\"\n            },\n            \"primary\": {\n              \"type\": \"boolean\"\n            }\n          },\n          \"required\": [\"id\"]\n        }\n      }\n    },\n    \"web\": {\n      \"type\": \"object\",\n      \"description\": \"Web-specific event\
  \ details.\",\n      \"properties\": {\n        \"webPageDetails\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"URL\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"siteSection\": {\n              \"type\": \"string\"\n            },\n            \"isHomePage\": {\n              \"type\": \"boolean\"\n            }\n          }\n        },\n        \"webInteraction\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"URL\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"download\", \"exit\", \"other\"]\n            }\n          }\n        },\n        \"webReferrer\": {\n          \"\
  type\": \"object\",\n          \"properties\": {\n            \"URL\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"internal\", \"external\", \"search_engine\", \"social\", \"typed_bookmarked\"]\n            }\n          }\n        }\n      }\n    },\n    \"commerce\": {\n      \"type\": \"object\",\n      \"description\": \"Commerce-specific event details.\",\n      \"properties\": {\n        \"purchases\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"number\"\n            }\n          }\n        },\n        \"order\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"purchaseID\": {\n              \"type\": \"string\"\n            },\n            \"currencyCode\": {\n              \"type\": \"string\"\n            },\n            \"priceTotal\": {\n  \
  \            \"type\": \"number\"\n            },\n            \"payments\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"paymentType\": {\n                    \"type\": \"string\"\n                  },\n                  \"paymentAmount\": {\n                    \"type\": \"number\"\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"productListItems\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"SKU\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"quantity\": {\n                \"type\": \"integer\"\n              },\n              \"priceTotal\": {\n                \"type\": \"number\"\n              },\n   \
  \           \"currencyCode\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"device\": {\n      \"type\": \"object\",\n      \"description\": \"The device used during the event.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"mobile\", \"tablet\", \"desktop\", \"ereader\", \"gaming\", \"television\", \"settop\", \"mediaplayer\"]\n        },\n        \"manufacturer\": {\n          \"type\": \"string\"\n        },\n        \"model\": {\n          \"type\": \"string\"\n        },\n        \"screenHeight\": {\n          \"type\": \"integer\"\n        },\n        \"screenWidth\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"environment\": {\n      \"type\": \"object\",\n      \"description\": \"Environment details at the time of the event.\",\n      \"properties\": {\n        \"browserDetails\": {\n          \"type\": \"object\",\n     \
  \     \"properties\": {\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"version\": {\n              \"type\": \"string\"\n            },\n            \"userAgent\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"operatingSystem\": {\n          \"type\": \"string\"\n        },\n        \"operatingSystemVersion\": {\n          \"type\": \"string\"\n        },\n        \"ipV4\": {\n          \"type\": \"string\",\n          \"format\": \"ipv4\"\n        }\n      }\n    },\n    \"source\": {\n      \"type\": \"object\",\n      \"description\": \"The source system that generated the event.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the source product or system.\"\n        },\n        \"datasetId\": {\n          \"type\": \"string\",\n          \"description\": \"The Experience Platform dataset ID where this event is stored.\"\n\
  \        }\n      }\n    }\n  },\n  \"required\": [\"eventId\", \"eventType\", \"timestamp\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/adobe-experience-cloud-event.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Adobe Experience Cloud Event
---
