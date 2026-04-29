---
description: Information about a site.
layout: schema
name: Site
properties_list:
- description: ''
  name: SiteId
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: SiteArn
  type: object
- description: ''
  name: Notes
  type: object
- description: ''
  name: OperatingAddressCountryCode
  type: object
- description: ''
  name: OperatingAddressStateOrRegion
  type: object
- description: ''
  name: OperatingAddressCity
  type: object
- description: ''
  name: RackPhysicalProperties
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-site-schema.json
slug: openapi-site
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-site-schema.json\",\n  \"title\": \"Site\",\n  \"description\": \"Information about a site.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SiteId\": {\n      \"$ref\": \"#/components/schemas/SiteId\"\n    },\n    \"AccountId\": {\n      \"$ref\": \"#/components/schemas/AccountId\"\n    },\n    \"Name\": {\n      \"$ref\": \"#/components/schemas/SiteName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/SiteDescription\"\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The site tags.\"\n        }\n      ]\n    },\n    \"SiteArn\": {\n      \"$ref\": \"#/components/schemas/SiteArn\"\n    },\n    \"Notes\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/SiteNotes\"\n        },\n        {\n          \"description\": \" Notes about a site. \"\n        }\n      ]\n    },\n    \"OperatingAddressCountryCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountryCode\"\n        },\n        {\n          \"description\": \" The ISO-3166 two-letter country code where the hardware is installed and powered on. \"\n        }\n      ]\n    },\n    \"OperatingAddressStateOrRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateOrRegion\"\n        },\n        {\n          \"description\": \" State or region where the hardware is installed and powered on. \"\n        }\n      ]\n    },\n    \"OperatingAddressCity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/City\"\n        },\n        {\n          \"description\": \" City where the hardware is installed and powered on. \"\n        }\n      ]\n    },\n    \"RackPhysicalProperties\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RackPhysicalProperties\"\n        },\n        {\n          \"description\": \" Information about the physical and logistical details for a rack at the site. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-site-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: Site
---
