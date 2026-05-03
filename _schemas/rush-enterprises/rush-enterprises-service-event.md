---
description: A service event for a commercial vehicle managed through RushCare Service Connect
layout: schema
name: Rush Enterprises Service Event
properties_list:
- description: Unique service event identifier
  name: eventId
  type: string
- description: Vehicle associated with this service event
  name: vehicleId
  type: string
- description: Vehicle VIN
  name: vin
  type: string
- description: Type of service
  name: serviceType
  type: string
- description: Current service status
  name: status
  type: string
- description: ''
  name: location
  type: object
- description: When the service is scheduled
  name: scheduledDate
  type: string
- description: When the service was completed
  name: completedDate
  type: string
- description: Telematics fault codes from Geotab
  name: faultCodes
  type: array
- description: Service notes or description
  name: notes
  type: string
provider_name: Rush Enterprises
provider_slug: rush-enterprises
schema_file: json-schema/rush-enterprises-service-event-schema.json
slug: rush-enterprises-service-event
source_filename: rush-enterprises-service-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://api-evangelist.github.io/rush-enterprises/json-schema/rush-enterprises-service-event-schema.json\",\n  \"title\": \"Rush Enterprises Service Event\",\n  \"description\": \"A service event for a commercial vehicle managed through RushCare Service Connect\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique service event identifier\"\n    },\n    \"vehicleId\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle associated with this service event\"\n    },\n    \"vin\": {\n      \"type\": \"string\",\n      \"description\": \"Vehicle VIN\"\n    },\n    \"serviceType\": {\n      \"type\": \"string\",\n      \"enum\": [\"preventive_maintenance\", \"repair\", \"inspection\", \"emergency\"],\n      \"description\": \"Type of service\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"\
  scheduled\", \"in_progress\", \"completed\", \"cancelled\"],\n      \"description\": \"Current service status\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"locationId\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"address\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"scheduledDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the service is scheduled\"\n    },\n    \"completedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the service was completed\"\n    },\n    \"faultCodes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Telematics\
  \ fault codes from Geotab\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Service notes or description\"\n    }\n  },\n  \"required\": [\"eventId\", \"vehicleId\", \"serviceType\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rush-enterprises/refs/heads/main/json-schema/rush-enterprises-service-event-schema.json
tags:
- Commercial Vehicles
- Fleet Management
- Telematics
- Truck Dealerships
- Transportation
title: Rush Enterprises Service Event
---
