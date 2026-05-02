---
description: Schema representing a physical site or location managed by Juniper platforms such as Mist and Junos Space. A site is a logical grouping of network devices at a physical location such as a building, campus, or data center.
layout: schema
name: Juniper Site
properties_list:
- description: Unique site identifier
  name: id
  type: string
- description: Site name
  name: name
  type: string
- description: Organization this site belongs to
  name: org_id
  type: string
- description: Physical street address
  name: address
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country_code
  type: string
- description: IANA timezone name (e.g., America/Los_Angeles)
  name: timezone
  type: string
- description: ''
  name: latlng
  type: object
- description: Site group identifiers this site belongs to
  name: site_groups
  type: array
- description: Count of devices by type at this site
  name: device_counts
  type: object
- description: Floorplan maps associated with the site
  name: maps
  type: array
- description: Radio frequency template applied to this site
  name: rf_template_id
  type: string
- description: Network template applied to this site
  name: network_template_id
  type: string
- description: Site-specific settings
  name: settings
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Juniper Networks
provider_slug: juniper
schema_file: json-schema/juniper-site.json
slug: juniper-site
source_filename: juniper-site.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/juniper/json-schema/juniper-site.json\",\n  \"title\": \"Juniper Site\",\n  \"description\": \"Schema representing a physical site or location managed by Juniper platforms such as Mist and Junos Space. A site is a logical grouping of network devices at a physical location such as a building, campus, or data center.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique site identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Site name\"\n    },\n    \"org_id\": {\n      \"type\": \"string\",\n      \"description\": \"Organization this site belongs to\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Physical street address\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\":\
  \ \"string\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"minLength\": 2,\n      \"maxLength\": 2,\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"IANA timezone name (e.g., America/Los_Angeles)\"\n    },\n    \"latlng\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lat\": {\n          \"type\": \"number\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"lng\": {\n          \"type\": \"number\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        }\n      },\n      \"required\": [\"lat\", \"lng\"]\n    },\n    \"site_groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Site group identifiers this site belongs to\"\n    },\n    \"device_counts\": {\n      \"type\": \"object\",\n      \"description\": \"Count of devices by type at\
  \ this site\",\n      \"properties\": {\n        \"access_points\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"switches\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"gateways\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        },\n        \"wan_edges\": {\n          \"type\": \"integer\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"maps\": {\n      \"type\": \"array\",\n      \"description\": \"Floorplan maps associated with the site\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"width\": {\n            \"type\": \"number\",\n            \"description\": \"Width in meters\"\n          },\n          \"height\": {\n            \"type\": \"number\",\n            \"description\": \"Height\
  \ in meters\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL to the floorplan image\"\n          }\n        }\n      }\n    },\n    \"rf_template_id\": {\n      \"type\": \"string\",\n      \"description\": \"Radio frequency template applied to this site\"\n    },\n    \"network_template_id\": {\n      \"type\": \"string\",\n      \"description\": \"Network template applied to this site\"\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Site-specific settings\",\n      \"properties\": {\n        \"auto_upgrade\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether automatic firmware upgrades are enabled\"\n        },\n        \"rtsa\": {\n          \"type\": \"object\",\n          \"description\": \"Real-Time Status and Analytics settings\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\"\n \
  \           }\n          }\n        }\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/json-schema/juniper-site.json
tags:
- AI
- Automation
- Cloud
- Enterprise
- Networking
- SDN
- Security
title: Juniper Site
---
