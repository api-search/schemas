---
description: The most generic type of item in the Schema.org vocabulary. All other Schema.org types inherit from Thing.
layout: schema
name: Schema.org Thing
properties_list:
- description: The Schema.org type of the item.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the item.
  name: name
  type: string
- description: A description of the item.
  name: description
  type: string
- description: URL of the item.
  name: url
  type: string
- description: An image of the item.
  name: image
  type: object
- description: The identifier property represents any kind of identifier for any kind of Thing.
  name: identifier
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
- description: An alias for the item.
  name: alternateName
  type: string
- description: An additional type for the item, typically used for adding more specific types from external vocabularies.
  name: additionalType
  type: string
- description: Indicates a page for which this thing is the main entity being described.
  name: mainEntityOfPage
  type: object
- description: Indicates a potential Action, which describes an idealized action in which this thing would play an 'object' role.
  name: potentialAction
  type: object
- description: A CreativeWork or Event about this Thing.
  name: subjectOf
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-thing-schema.json
slug: schema-org-thing
source_filename: schema-org-thing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/thing.json\",\n  \"title\": \"Schema.org Thing\",\n  \"description\": \"The most generic type of item in the Schema.org vocabulary. All other Schema.org types inherit from Thing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type of the item.\",\n      \"const\": \"Thing\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the item.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the item.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the item.\"\n    },\n   \
  \ \"image\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of an image of the item.\"\n        },\n        {\n          \"$ref\": \"#/$defs/ImageObject\"\n        }\n      ],\n      \"description\": \"An image of the item.\"\n    },\n    \"identifier\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"$ref\": \"#/$defs/PropertyValue\"\n        }\n      ],\n      \"description\": \"The identifier property represents any kind of identifier for any kind of Thing.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's\
  \ identity.\"\n    },\n    \"alternateName\": {\n      \"type\": \"string\",\n      \"description\": \"An alias for the item.\"\n    },\n    \"additionalType\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"An additional type for the item, typically used for adding more specific types from external vocabularies.\"\n    },\n    \"mainEntityOfPage\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        {\n          \"$ref\": \"#/$defs/CreativeWork\"\n        }\n      ],\n      \"description\": \"Indicates a page for which this thing is the main entity being described.\"\n    },\n    \"potentialAction\": {\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/$defs/Action\"\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Action\"\n          }\n        }\n      ],\n      \"description\": \"Indicates a potential Action, which\
  \ describes an idealized action in which this thing would play an 'object' role.\"\n    },\n    \"subjectOf\": {\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/$defs/CreativeWork\"\n        },\n        {\n          \"$ref\": \"#/$defs/Event\"\n        }\n      ],\n      \"description\": \"A CreativeWork or Event about this Thing.\"\n    }\n  },\n  \"$defs\": {\n    \"ImageObject\": {\n      \"type\": \"object\",\n      \"description\": \"An image file.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"const\": \"ImageObject\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the image.\"\n        },\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"The width of the image in pixels.\"\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"The height of the image in pixels.\"\
  \n        },\n        \"caption\": {\n          \"type\": \"string\",\n          \"description\": \"The caption for this image.\"\n        }\n      }\n    },\n    \"PropertyValue\": {\n      \"type\": \"object\",\n      \"description\": \"A property-value pair representing an explicit or inferred attribute of a Thing.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"const\": \"PropertyValue\"\n        },\n        \"propertyID\": {\n          \"type\": \"string\",\n          \"description\": \"A commonly used identifier for the characteristic represented by the property.\"\n        },\n        \"value\": {\n          \"description\": \"The value of the property.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the property.\"\n        }\n      }\n    },\n    \"CreativeWork\": {\n      \"type\": \"object\",\n      \"description\": \"The most generic kind of creative work, including\
  \ books, movies, photographs, software programs, etc.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"const\": \"CreativeWork\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the creative work.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the creative work.\"\n        }\n      }\n    },\n    \"Action\": {\n      \"type\": \"object\",\n      \"description\": \"An action performed by a direct agent and indirect participants upon a direct object.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of action.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the action.\"\n        },\n        \"target\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\
  ,\n          \"description\": \"Indicates a target EntryPoint for an Action.\"\n        }\n      }\n    },\n    \"Event\": {\n      \"type\": \"object\",\n      \"description\": \"An event happening at a certain time and location.\",\n      \"properties\": {\n        \"@type\": {\n          \"type\": \"string\",\n          \"const\": \"Event\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the event.\"\n        },\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The start date and time of the event.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-thing-schema.json
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
title: Schema.org Thing
---
