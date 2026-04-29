---
description: CreateSiteInput schema from Amazon Outposts
layout: schema
name: CreateSiteInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Notes
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: OperatingAddress
  type: object
- description: ''
  name: ShippingAddress
  type: object
- description: ''
  name: RackPhysicalProperties
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-create-site-input-schema.json
slug: openapi-create-site-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-create-site-input-schema.json\",\n  \"title\": \"CreateSiteInput\",\n  \"description\": \"CreateSiteInput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"$ref\": \"#/components/schemas/SiteName\"\n    },\n    \"Description\": {\n      \"$ref\": \"#/components/schemas/SiteDescription\"\n    },\n    \"Notes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SiteNotes\"\n        },\n        {\n          \"description\": \"Additional information that you provide about site access requirements, electrician scheduling, personal protective equipment, or regulation of equipment materials that could affect your installation process. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \" The tags to apply to a site. \"\n        }\n      ]\n    },\n    \"OperatingAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Address\"\n        },\n        {\n          \"description\": \" The location to install and power on the hardware. This address might be different from the shipping address. \"\n        }\n      ]\n    },\n    \"ShippingAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Address\"\n        },\n        {\n          \"description\": \" The location to ship the hardware. This address might be different from the operating address. \"\n        }\n      ]\n    },\n    \"RackPhysicalProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RackPhysicalProperties\"\n        },\n        {\n          \"description\": \" Information about the physical and logistical details\
  \ for the rack at this site. For more information about hardware requirements for racks, see <a href=\\\"https://docs.aws.amazon.com/outposts/latest/userguide/outposts-requirements.html#checklist\\\">Network readiness checklist</a> in the Amazon Web Services Outposts User Guide. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-create-site-input-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: CreateSiteInput
---
