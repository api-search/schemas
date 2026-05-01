---
description: Schema representing an ocean shipping booking and tracking record in the INTTRA e2open platform.
layout: schema
name: e2open / INTTRA Ocean Shipment
properties_list:
- description: INTTRA booking reference identifier
  name: bookingId
  type: string
- description: Ocean carrier's own booking reference number
  name: carrierBookingReference
  type: string
- description: Ocean carrier SCAC code
  name: carrier
  type: string
- description: Full name of the ocean carrier
  name: carrierName
  type: string
- description: Current booking status
  name: status
  type: string
- description: Port of loading (POL)
  name: originPort
  type: object
- description: Port of discharge (POD)
  name: destinationPort
  type: object
- description: Estimated time of departure
  name: etd
  type: string
- description: Estimated time of arrival
  name: eta
  type: string
- description: ''
  name: vessel
  type: object
- description: Vessel voyage number
  name: voyage
  type: string
- description: ''
  name: shipper
  type: object
- description: ''
  name: consignee
  type: object
- description: ''
  name: notifyParty
  type: object
- description: List of containers in this booking
  name: containers
  type: array
- description: Commodity description
  name: commodity
  type: string
- description: Harmonized System tariff code
  name: hsCode
  type: string
- description: ''
  name: submittedAt
  type: string
- description: ''
  name: confirmedAt
  type: string
provider_name: e2open
provider_slug: e2open
schema_file: json-schema/e2open-shipment-schema.json
slug: e2open-shipment
source_filename: e2open-shipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.inttra.com/v1/schemas/shipment\",\n  \"title\": \"e2open / INTTRA Ocean Shipment\",\n  \"description\": \"Schema representing an ocean shipping booking and tracking record in the INTTRA e2open platform.\",\n  \"type\": \"object\",\n  \"required\": [\"bookingId\", \"carrier\", \"originPort\", \"destinationPort\", \"status\"],\n  \"properties\": {\n    \"bookingId\": {\n      \"type\": \"string\",\n      \"description\": \"INTTRA booking reference identifier\"\n    },\n    \"carrierBookingReference\": {\n      \"type\": \"string\",\n      \"description\": \"Ocean carrier's own booking reference number\"\n    },\n    \"carrier\": {\n      \"type\": \"string\",\n      \"description\": \"Ocean carrier SCAC code\",\n      \"examples\": [\"MAEU\", \"MSCU\", \"CMDU\", \"HLCU\", \"EGLV\"],\n      \"minLength\": 4,\n      \"maxLength\": 4\n    },\n    \"carrierName\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Full name of the ocean carrier\",\n      \"examples\": [\"Maersk\", \"MSC\", \"CMA CGM\", \"Hapag-Lloyd\", \"Evergreen\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current booking status\",\n      \"enum\": [\"PENDING\", \"CONFIRMED\", \"CANCELLED\", \"AMENDED\", \"COMPLETED\"]\n    },\n    \"originPort\": {\n      \"$ref\": \"#/$defs/Port\",\n      \"description\": \"Port of loading (POL)\"\n    },\n    \"destinationPort\": {\n      \"$ref\": \"#/$defs/Port\",\n      \"description\": \"Port of discharge (POD)\"\n    },\n    \"etd\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Estimated time of departure\"\n    },\n    \"eta\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Estimated time of arrival\"\n    },\n    \"vessel\": {\n      \"$ref\": \"#/$defs/Vessel\"\n    },\n    \"voyage\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Vessel voyage number\"\n    },\n    \"shipper\": {\n      \"$ref\": \"#/$defs/TradeParty\"\n    },\n    \"consignee\": {\n      \"$ref\": \"#/$defs/TradeParty\"\n    },\n    \"notifyParty\": {\n      \"$ref\": \"#/$defs/TradeParty\"\n    },\n    \"containers\": {\n      \"type\": \"array\",\n      \"description\": \"List of containers in this booking\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Container\"\n      }\n    },\n    \"commodity\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity description\"\n    },\n    \"hsCode\": {\n      \"type\": \"string\",\n      \"description\": \"Harmonized System tariff code\",\n      \"pattern\": \"^[0-9]{4,10}$\"\n    },\n    \"submittedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"confirmedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"Port\": {\n      \"type\": \"object\",\n      \"required\": [\"portCode\"],\n      \"\
  properties\": {\n        \"portCode\": {\n          \"type\": \"string\",\n          \"description\": \"UN/LOCODE port code (e.g., USLAX, CNSHA)\",\n          \"pattern\": \"^[A-Z]{2}[A-Z0-9]{3}$\"\n        },\n        \"portName\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"terminal\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Vessel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"vesselName\": {\n          \"type\": \"string\"\n        },\n        \"imoNumber\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{7}$\",\n          \"description\": \"IMO vessel identification number\"\n        },\n        \"callSign\": {\n          \"type\": \"string\"\n        },\n        \"flag\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        }\n      }\n    },\n    \"TradeParty\"\
  : {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"address\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        },\n        \"phone\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Container\": {\n      \"type\": \"object\",\n      \"required\": [\"containerType\"],\n      \"properties\": {\n        \"containerNumber\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 6346 container number\",\n          \"pattern\": \"^[A-Z]{4}[0-9]{7}$\"\
  \n        },\n        \"containerType\": {\n          \"type\": \"string\",\n          \"description\": \"ISO container type code\",\n          \"enum\": [\"20GP\", \"40GP\", \"40HC\", \"45HC\", \"20RF\", \"40RF\", \"20OT\", \"40OT\", \"20FR\", \"40FR\"]\n        },\n        \"sealNumber\": {\n          \"type\": \"string\"\n        },\n        \"tare\": {\n          \"type\": \"number\",\n          \"description\": \"Container tare weight in kg\"\n        },\n        \"grossWeightKg\": {\n          \"type\": \"number\",\n          \"description\": \"Total gross weight including cargo in kg\",\n          \"minimum\": 0\n        },\n        \"cargoWeightKg\": {\n          \"type\": \"number\",\n          \"description\": \"Net cargo weight in kg\",\n          \"minimum\": 0\n        },\n        \"vgm\": {\n          \"type\": \"number\",\n          \"description\": \"Verified gross mass in kg (SOLAS requirement)\",\n          \"minimum\": 0\n        },\n        \"hazmat\": {\n         \
  \ \"type\": \"boolean\",\n          \"description\": \"Whether container carries hazardous materials\",\n          \"default\": false\n        },\n        \"refrigerated\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether container is a refrigerated unit\",\n          \"default\": false\n        },\n        \"setTemperatureCelsius\": {\n          \"type\": \"number\",\n          \"description\": \"Required temperature for refrigerated containers\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/e2open/refs/heads/main/json-schema/e2open-shipment-schema.json
tags: []
title: e2open / INTTRA Ocean Shipment
---
