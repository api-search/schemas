---
description: Schema representing a vessel in the DNV classification register, including class status, certificates, and survey records.
layout: schema
name: DNV Classified Vessel
properties_list:
- description: IMO vessel identification number assigned by the International Maritime Organization
  name: imoNumber
  type: string
- description: Registered name of the vessel
  name: vesselName
  type: string
- description: Vessel radio call sign
  name: callSign
  type: string
- description: ISO 3166-1 alpha-2 country code for the flag state
  name: flagState
  type: string
- description: DNV ship type classification
  name: shipType
  type: string
- description: Current classification status
  name: classStatus
  type: string
- description: Full DNV class notation string (e.g., 1A1 Tanker ESP CSR)
  name: classNotation
  type: string
- description: Legal vessel owner name
  name: vesselOwner
  type: string
- description: Technical management company name
  name: technicalManager
  type: string
- description: ''
  name: physicalDimensions
  type: object
- description: ''
  name: tonnage
  type: object
- description: ''
  name: buildInfo
  type: object
- description: ''
  name: propulsion
  type: object
- description: ''
  name: surveys
  type: object
- description: Active classification and statutory certificates
  name: certificates
  type: array
provider_name: DNV
provider_slug: dnv
schema_file: json-schema/dnv-vessel-schema.json
slug: dnv-vessel
source_filename: dnv-vessel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://maritime.dnv.com/api/cs-iacs-customer/schemas/vessel\",\n  \"title\": \"DNV Classified Vessel\",\n  \"description\": \"Schema representing a vessel in the DNV classification register, including class status, certificates, and survey records.\",\n  \"type\": \"object\",\n  \"required\": [\"imoNumber\", \"vesselName\", \"classStatus\"],\n  \"properties\": {\n    \"imoNumber\": {\n      \"type\": \"string\",\n      \"description\": \"IMO vessel identification number assigned by the International Maritime Organization\",\n      \"pattern\": \"^[0-9]{7}$\"\n    },\n    \"vesselName\": {\n      \"type\": \"string\",\n      \"description\": \"Registered name of the vessel\",\n      \"maxLength\": 100\n    },\n    \"callSign\": {\n      \"type\": \"string\",\n      \"description\": \"Vessel radio call sign\"\n    },\n    \"flagState\": {\n      \"type\": \"string\",\n      \"description\": \"\
  ISO 3166-1 alpha-2 country code for the flag state\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"shipType\": {\n      \"type\": \"string\",\n      \"description\": \"DNV ship type classification\",\n      \"examples\": [\"General Cargo\", \"Bulk Carrier\", \"Tanker\", \"Container\", \"VLCC\", \"LNG Carrier\", \"Cruise Ship\", \"RORO\"]\n    },\n    \"classStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current classification status\",\n      \"enum\": [\"CLASSED\", \"SUSPENDED\", \"WITHDRAWN\", \"DELETED\"]\n    },\n    \"classNotation\": {\n      \"type\": \"string\",\n      \"description\": \"Full DNV class notation string (e.g., 1A1 Tanker ESP CSR)\",\n      \"examples\": [\"1A1 Tanker ESP CSR\", \"1A1 BulkCarrier ESP CSR\", \"1A1 ContainerShip CSR\"]\n    },\n    \"vesselOwner\": {\n      \"type\": \"string\",\n      \"description\": \"Legal vessel owner name\"\n    },\n    \"technicalManager\": {\n      \"type\": \"string\",\n      \"description\": \"Technical\
  \ management company name\"\n    },\n    \"physicalDimensions\": {\n      \"$ref\": \"#/$defs/VesselDimensions\"\n    },\n    \"tonnage\": {\n      \"$ref\": \"#/$defs/VesselTonnage\"\n    },\n    \"buildInfo\": {\n      \"$ref\": \"#/$defs/BuildInfo\"\n    },\n    \"propulsion\": {\n      \"$ref\": \"#/$defs/PropulsionInfo\"\n    },\n    \"surveys\": {\n      \"$ref\": \"#/$defs/SurveySummary\"\n    },\n    \"certificates\": {\n      \"type\": \"array\",\n      \"description\": \"Active classification and statutory certificates\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Certificate\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"VesselDimensions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lengthOverall\": {\n          \"type\": \"number\",\n          \"description\": \"Length overall in meters\",\n          \"minimum\": 0\n        },\n        \"lengthBetweenPerpendiculars\": {\n          \"type\": \"number\",\n          \"description\": \"Length between\
  \ perpendiculars in meters\",\n          \"minimum\": 0\n        },\n        \"beam\": {\n          \"type\": \"number\",\n          \"description\": \"Moulded breadth in meters\",\n          \"minimum\": 0\n        },\n        \"depth\": {\n          \"type\": \"number\",\n          \"description\": \"Moulded depth in meters\",\n          \"minimum\": 0\n        },\n        \"draught\": {\n          \"type\": \"number\",\n          \"description\": \"Maximum design draught in meters\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"VesselTonnage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"grossTonnage\": {\n          \"type\": \"number\",\n          \"description\": \"Gross tonnage (GT) per ITC 1969\",\n          \"minimum\": 0\n        },\n        \"netTonnage\": {\n          \"type\": \"number\",\n          \"description\": \"Net tonnage (NT) per ITC 1969\",\n          \"minimum\": 0\n        },\n        \"deadweightTonnage\": {\n          \"\
  type\": \"number\",\n          \"description\": \"Deadweight tonnage (DWT) in metric tons\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"BuildInfo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"buildYear\": {\n          \"type\": \"integer\",\n          \"description\": \"Year vessel was built\",\n          \"minimum\": 1800,\n          \"maximum\": 2100\n        },\n        \"shipyard\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the shipyard where vessel was built\"\n        },\n        \"shipyardCountry\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"hullNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Shipyard hull construction number\"\n        },\n        \"hullMaterial\": {\n          \"type\": \"string\",\n          \"enum\": [\"STEEL\", \"ALUMINUM\", \"GRP\", \"WOOD\", \"COMPOSITE\"]\n        }\n      }\n    },\n    \"PropulsionInfo\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"engineType\": {\n          \"type\": \"string\",\n          \"examples\": [\"2-stroke diesel\", \"4-stroke diesel\", \"Gas turbine\", \"Electric\", \"LNG dual-fuel\"]\n        },\n        \"engineMake\": {\n          \"type\": \"string\"\n        },\n        \"enginePowerKW\": {\n          \"type\": \"number\",\n          \"description\": \"Main engine output in kilowatts\",\n          \"minimum\": 0\n        },\n        \"numberOfEngines\": {\n          \"type\": \"integer\",\n          \"minimum\": 1\n        },\n        \"propellerType\": {\n          \"type\": \"string\",\n          \"enum\": [\"FIXED_PITCH\", \"CONTROLLABLE_PITCH\", \"AZIMUTH_THRUSTER\", \"VOITH_SCHNEIDER\"]\n        }\n      }\n    },\n    \"SurveySummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"lastAnnualSurveyDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"nextAnnualSurveyDue\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"lastIntermediateSurveyDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"nextIntermediateSurveyDue\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"lastSpecialSurveyDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"nextSpecialSurveyDue\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"continuousSurveyMachinery\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"Certificate\": {\n      \"type\": \"object\",\n      \"required\": [\"certificateType\", \"status\"],\n      \"properties\": {\n        \"certificateId\": {\n          \"type\": \"string\"\n        },\n        \"certificateType\": {\n          \"type\": \"string\",\n          \"enum\": [\"CLASS\", \"STATUTORY\", \"SURVEY_REPORT\", \"ENTRY_IN_CLASS\"\
  ]\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Full certificate title\"\n        },\n        \"issueDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"expiryDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"VALID\", \"EXPIRED\", \"WITHDRAWN\"]\n        },\n        \"issuingOffice\": {\n          \"type\": \"string\",\n          \"description\": \"DNV office that issued the certificate\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dnv/refs/heads/main/json-schema/dnv-vessel-schema.json
tags:
- Maritime
- Energy
- Classification
- Vessel
- Data Platform
title: DNV Classified Vessel
---
