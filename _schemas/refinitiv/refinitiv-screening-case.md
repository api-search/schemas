---
description: Represents a screening case in the World-Check One API, containing entity information, screening configuration, and matched results for KYC and due diligence workflows.
layout: schema
name: Refinitiv World-Check Screening Case
properties_list:
- description: System-generated unique identifier for the case.
  name: caseSystemId
  type: string
- description: Client-defined case identifier for tracking purposes.
  name: caseId
  type:
  - string
  - 'null'
- description: The group under which the case is created, defining screening parameters and resolution toolkit.
  name: groupId
  type: string
- description: The type of entity being screened.
  name: entityType
  type: string
- description: Provider types to screen against. WATCHLIST corresponds to World-Check risk intelligence data.
  name: providerTypes
  type: array
- description: Name information for the entity being screened.
  name: name
  type: object
- description: Additional fields for improving match accuracy.
  name: secondaryFields
  type:
  - object
  - 'null'
- description: The screening state for each provider type.
  name: caseScreeningState
  type:
  - object
  - 'null'
- description: Date and time the case was created.
  name: creationDate
  type: string
- description: Date and time the case was last modified.
  name: modificationDate
  type: string
- description: Screening results matched against the entity.
  name: results
  type:
  - array
  - 'null'
provider_name: Refinitiv
provider_slug: refinitiv
schema_file: json-schema/refinitiv-screening-case-schema.json
slug: refinitiv-screening-case
source_filename: refinitiv-screening-case-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.refinitiv.com/schemas/refinitiv/screening-case.json\",\n  \"title\": \"Refinitiv World-Check Screening Case\",\n  \"description\": \"Represents a screening case in the World-Check One API, containing entity information, screening configuration, and matched results for KYC and due diligence workflows.\",\n  \"type\": \"object\",\n  \"required\": [\"groupId\", \"entityType\", \"name\"],\n  \"properties\": {\n    \"caseSystemId\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated unique identifier for the case.\"\n    },\n    \"caseId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Client-defined case identifier for tracking purposes.\",\n      \"maxLength\": 255\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"The group under which the case is created, defining screening parameters and resolution toolkit.\"\
  \n    },\n    \"entityType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of entity being screened.\",\n      \"enum\": [\"INDIVIDUAL\", \"ORGANISATION\", \"VESSEL\"]\n    },\n    \"providerTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"WATCHLIST\", \"CLIENT_WATCHLIST\", \"MEDIA_CHECK\", \"PASSPORT_CHECK\"]\n      },\n      \"description\": \"Provider types to screen against. WATCHLIST corresponds to World-Check risk intelligence data.\"\n    },\n    \"name\": {\n      \"type\": \"object\",\n      \"description\": \"Name information for the entity being screened.\",\n      \"properties\": {\n        \"firstName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"First name of the individual.\",\n          \"maxLength\": 255\n        },\n        \"middleName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Middle name of the individual.\",\n \
  \         \"maxLength\": 255\n        },\n        \"lastName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Last name of the individual.\",\n          \"maxLength\": 255\n        },\n        \"fullName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Full name, used when parts are not available or for organization names.\",\n          \"maxLength\": 1000\n        }\n      }\n    },\n    \"secondaryFields\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Additional fields for improving match accuracy.\",\n      \"properties\": {\n        \"dateOfBirth\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Date of birth for individual screening.\"\n        },\n        \"countryLocation\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Country of location, ISO 3166-1 alpha-2 code.\",\n          \"pattern\": \"^[A-Z]{2}$\"\
  \n        },\n        \"nationality\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Nationality, ISO 3166-1 alpha-2 code.\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"gender\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Gender of the individual.\",\n          \"enum\": [\"MALE\", \"FEMALE\", \"UNSPECIFIED\", null]\n        },\n        \"placeOfBirth\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Place of birth.\"\n        },\n        \"registeredCountry\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Registered country for organizations.\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        }\n      }\n    },\n    \"caseScreeningState\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The screening state for each provider type.\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"enum\": [\"INITIAL\"\
  , \"ONGOING\"]\n      }\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the case was created.\"\n    },\n    \"modificationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the case was last modified.\"\n    },\n    \"results\": {\n      \"type\": [\"array\", \"null\"],\n      \"items\": {\n        \"$ref\": \"#/$defs/ScreeningResult\"\n      },\n      \"description\": \"Screening results matched against the entity.\"\n    }\n  },\n  \"$defs\": {\n    \"ScreeningResult\": {\n      \"type\": \"object\",\n      \"description\": \"A single screening match result from the World-Check database.\",\n      \"properties\": {\n        \"resultId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the screening result.\"\n        },\n        \"referenceId\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"World-Check reference profile identifier.\"\n        },\n        \"matchStrength\": {\n          \"type\": \"string\",\n          \"description\": \"Strength of the match between submitted and matched terms.\",\n          \"enum\": [\"EXACT\", \"STRONG\", \"MEDIUM\", \"WEAK\"]\n        },\n        \"matchedTerm\": {\n          \"type\": \"string\",\n          \"description\": \"The name or term that was matched from the World-Check database.\"\n        },\n        \"submittedTerm\": {\n          \"type\": \"string\",\n          \"description\": \"The original term submitted for screening.\"\n        },\n        \"matchedNameType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of name matched such as PRIMARY or ALIAS.\",\n          \"enum\": [\"PRIMARY\", \"AKA\", \"DBA\", \"FKA\", \"MAIDEN\"]\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\"\
  : \"Risk categories such as PEP, Sanctions, Adverse Media, or Law Enforcement.\"\n        },\n        \"resolution\": {\n          \"oneOf\": [\n            { \"$ref\": \"#/$defs/Resolution\" },\n            { \"type\": \"null\" }\n          ],\n          \"description\": \"The resolution status, null if unresolved.\"\n        },\n        \"providerType\": {\n          \"type\": \"string\",\n          \"description\": \"The provider that generated the match.\",\n          \"enum\": [\"WATCHLIST\", \"CLIENT_WATCHLIST\", \"MEDIA_CHECK\", \"PASSPORT_CHECK\"]\n        }\n      }\n    },\n    \"Resolution\": {\n      \"type\": \"object\",\n      \"description\": \"Resolution details for a screening result.\",\n      \"properties\": {\n        \"statusId\": {\n          \"type\": \"string\",\n          \"description\": \"The resolution status identifier from the resolution toolkit.\"\n        },\n        \"statusLabel\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\"\
  : \"Human-readable label for the resolution status.\"\n        },\n        \"riskId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The risk level identifier.\"\n        },\n        \"riskLabel\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Human-readable label for the risk level.\"\n        },\n        \"reasonId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The resolution reason identifier.\"\n        },\n        \"reasonLabel\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Human-readable label for the reason.\"\n        },\n        \"remarks\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Free-text remarks or notes.\"\n        },\n        \"resolvedDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date and time the result was resolved.\"\n        },\n        \"resolvedBy\"\
  : {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The user who resolved the result.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/json-schema/refinitiv-screening-case-schema.json
tags: []
title: Refinitiv World-Check Screening Case
---
