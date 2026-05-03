---
description: A software application.
layout: schema
name: Schema.org SoftwareApplication
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the application.
  name: name
  type: string
- description: A description of the application.
  name: description
  type: string
- description: URL of the application.
  name: url
  type: string
- description: An image of the application.
  name: image
  type: object
- description: Type of software application (e.g., GameApplication, SocialNetworkingApplication).
  name: applicationCategory
  type: string
- description: Subcategory of the application.
  name: applicationSubCategory
  type: string
- description: Operating systems supported (e.g., Windows, macOS, Android, iOS).
  name: operatingSystem
  type: string
- description: The name of the application suite to which the application belongs.
  name: applicationSuite
  type: string
- description: Version of the software instance.
  name: softwareVersion
  type: string
- description: Component dependency requirements for the software.
  name: softwareRequirements
  type: string
- description: Additional content for a software application.
  name: softwareAddOn
  type: object
- description: URL to download the application.
  name: downloadUrl
  type: string
- description: URL at which the app may be installed.
  name: installUrl
  type: string
- description: Features or content items that are part of this application.
  name: featureList
  type: object
- description: A link to a screenshot image of the app.
  name: screenshot
  type: object
- description: Permission(s) required by the application.
  name: permissions
  type: string
- description: Processor architecture required to run the application.
  name: processorRequirements
  type: string
- description: Minimum memory requirements.
  name: memoryRequirements
  type: string
- description: Storage requirements.
  name: storageRequirements
  type: string
- description: Size of the application / package.
  name: fileSize
  type: string
- description: Description of what changed in this version.
  name: releaseNotes
  type: string
- description: Countries for which the application is supported.
  name: countriesSupported
  type: string
- description: Device required to run the application.
  name: availableOnDevice
  type: string
- description: The author of this application.
  name: author
  type: object
- description: Date of first publication.
  name: datePublished
  type: string
- description: An offer to provide this application.
  name: offers
  type: object
- description: The overall rating.
  name: aggregateRating
  type: object
- description: A review of the application.
  name: review
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-software-application-schema.json
slug: schema-org-software-application
source_filename: schema-org-software-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/software-application.json\",\n  \"title\": \"Schema.org SoftwareApplication\",\n  \"description\": \"A software application.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"SoftwareApplication\", \"MobileApplication\", \"VideoGame\", \"WebApplication\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the application.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the application.\"\
  \n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the application.\"\n    },\n    \"applicationCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Type of software application (e.g., GameApplication, SocialNetworkingApplication).\"\n    },\n    \"applicationSubCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Subcategory of the application.\"\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Operating systems supported (e.g., Windows, macOS, Android, iOS).\"\n    },\n    \"applicationSuite\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application suite to which the application belongs.\"\n    },\n    \"softwareVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the software instance.\"\n    },\n\
  \    \"softwareRequirements\": {\n      \"type\": \"string\",\n      \"description\": \"Component dependency requirements for the software.\"\n    },\n    \"softwareAddOn\": {\n      \"$ref\": \"#\",\n      \"description\": \"Additional content for a software application.\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the application.\"\n    },\n    \"installUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL at which the app may be installed.\"\n    },\n    \"featureList\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Features or content items that are part of this application.\"\n    },\n    \"screenshot\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\"\
  \ },\n        { \"type\": \"array\", \"items\": { \"oneOf\": [{ \"type\": \"string\", \"format\": \"uri\" }, { \"$ref\": \"schema-org-image-object-schema.json\" }] } }\n      ],\n      \"description\": \"A link to a screenshot image of the app.\"\n    },\n    \"permissions\": {\n      \"type\": \"string\",\n      \"description\": \"Permission(s) required by the application.\"\n    },\n    \"processorRequirements\": {\n      \"type\": \"string\",\n      \"description\": \"Processor architecture required to run the application.\"\n    },\n    \"memoryRequirements\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum memory requirements.\"\n    },\n    \"storageRequirements\": {\n      \"type\": \"string\",\n      \"description\": \"Storage requirements.\"\n    },\n    \"fileSize\": {\n      \"type\": \"string\",\n      \"description\": \"Size of the application / package.\"\n    },\n    \"releaseNotes\": {\n      \"type\": \"string\",\n      \"description\": \"Description of\
  \ what changed in this version.\"\n    },\n    \"countriesSupported\": {\n      \"type\": \"string\",\n      \"description\": \"Countries for which the application is supported.\"\n    },\n    \"availableOnDevice\": {\n      \"type\": \"string\",\n      \"description\": \"Device required to run the application.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The author of this application.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"offers\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-offer-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-offer-schema.json\" } }\n      ],\n      \"description\": \"An offer to provide this application.\"\n    },\n    \"aggregateRating\"\
  : {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A review of the application.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-software-application-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org SoftwareApplication
---
