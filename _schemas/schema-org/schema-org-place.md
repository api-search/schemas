---
description: Entities that have a somewhat fixed, physical extension. Includes locations, buildings, geographic features, and more.
layout: schema
name: Schema.org Place
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the place.
  name: name
  type: string
- description: A description of the place.
  name: description
  type: string
- description: URL of the place.
  name: url
  type: string
- description: An image of the place.
  name: image
  type: object
- description: Physical address of the place.
  name: address
  type: object
- description: The geo coordinates of the place.
  name: geo
  type: object
- description: The latitude of a location.
  name: latitude
  type: number
- description: The longitude of a location.
  name: longitude
  type: number
- description: The telephone number.
  name: telephone
  type: string
- description: The fax number.
  name: faxNumber
  type: string
- description: A URL to a map of the place.
  name: hasMap
  type: string
- description: The basic containment relation between a place and one that contains it.
  name: containedInPlace
  type: object
- description: The basic containment relation between a place and another that it contains.
  name: containsPlace
  type: object
- description: A flag to signal that the item is accessible for free.
  name: isAccessibleForFree
  type: boolean
- description: A flag to signal that the Place is open to public visitors.
  name: publicAccess
  type: boolean
- description: The opening hours of a certain place.
  name: openingHoursSpecification
  type: object
- description: A photograph of this place.
  name: photo
  type: object
- description: A review of the place.
  name: review
  type: object
- description: The overall rating, based on a collection of reviews or ratings.
  name: aggregateRating
  type: object
- description: An amenity feature of this accommodation.
  name: amenityFeature
  type: object
- description: The total number of individuals that may attend an event or venue.
  name: maximumAttendeeCapacity
  type: integer
- description: Indicates whether it is allowed to smoke in the place.
  name: smokingAllowed
  type: boolean
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
- description: The identifier property represents any kind of identifier.
  name: identifier
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-place-schema.json
slug: schema-org-place
source_filename: schema-org-place-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/place.json\",\n  \"title\": \"Schema.org Place\",\n  \"description\": \"Entities that have a somewhat fixed, physical extension. Includes locations, buildings, geographic features, and more.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"Place\", \"AdministrativeArea\", \"CivicStructure\", \"Landform\", \"LandmarksOrHistoricalBuildings\", \"Residence\", \"TouristAttraction\", \"Accommodation\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the place.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"A description of the place.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the place.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the place.\"\n    },\n    \"address\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"schema-org-postal-address-schema.json\" }\n      ],\n      \"description\": \"Physical address of the place.\"\n    },\n    \"geo\": {\n      \"$ref\": \"schema-org-geo-coordinates-schema.json\",\n      \"description\": \"The geo coordinates of the place.\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"The latitude of a location.\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n   \
  \   \"description\": \"The longitude of a location.\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    },\n    \"telephone\": {\n      \"type\": \"string\",\n      \"description\": \"The telephone number.\"\n    },\n    \"faxNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The fax number.\"\n    },\n    \"hasMap\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to a map of the place.\"\n    },\n    \"containedInPlace\": {\n      \"$ref\": \"#\",\n      \"description\": \"The basic containment relation between a place and one that contains it.\"\n    },\n    \"containsPlace\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"The basic containment relation between a place and another that it contains.\"\n    },\n    \"isAccessibleForFree\": {\n      \"type\": \"boolean\",\n      \"description\": \"A flag to signal that\
  \ the item is accessible for free.\"\n    },\n    \"publicAccess\": {\n      \"type\": \"boolean\",\n      \"description\": \"A flag to signal that the Place is open to public visitors.\"\n    },\n    \"openingHoursSpecification\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/OpeningHoursSpecification\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/OpeningHoursSpecification\" } }\n      ],\n      \"description\": \"The opening hours of a certain place.\"\n    },\n    \"photo\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-image-object-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-image-object-schema.json\" } }\n      ],\n      \"description\": \"A photograph of this place.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A\
  \ review of the place.\"\n    },\n    \"aggregateRating\": {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating, based on a collection of reviews or ratings.\"\n    },\n    \"amenityFeature\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/LocationFeatureSpecification\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/LocationFeatureSpecification\" } }\n      ],\n      \"description\": \"An amenity feature of this accommodation.\"\n    },\n    \"maximumAttendeeCapacity\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of individuals that may attend an event or venue.\"\n    },\n    \"smokingAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether it is allowed to smoke in the place.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\"\
  , \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier property represents any kind of identifier.\"\n    }\n  },\n  \"$defs\": {\n    \"OpeningHoursSpecification\": {\n      \"type\": \"object\",\n      \"description\": \"A structured value providing information about the opening hours of a place.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"OpeningHoursSpecification\" },\n        \"dayOfWeek\": {\n          \"type\": \"string\",\n          \"enum\": [\"Monday\", \"Tuesday\", \"Wednesday\", \"Thursday\", \"Friday\", \"Saturday\", \"Sunday\", \"PublicHolidays\"],\n          \"description\": \"The day of the week for which these opening hours are valid.\"\n        },\n        \"opens\": { \"type\": \"string\", \"pattern\": \"^\\\\d{2}:\\\\d{2}$\", \"description\"\
  : \"The opening hour (HH:MM format).\" },\n        \"closes\": { \"type\": \"string\", \"pattern\": \"^\\\\d{2}:\\\\d{2}$\", \"description\": \"The closing hour (HH:MM format).\" },\n        \"validFrom\": { \"type\": \"string\", \"format\": \"date\", \"description\": \"The date when the opening hours become valid.\" },\n        \"validThrough\": { \"type\": \"string\", \"format\": \"date\", \"description\": \"The date after which the opening hours are no longer valid.\" }\n      }\n    },\n    \"LocationFeatureSpecification\": {\n      \"type\": \"object\",\n      \"description\": \"Specifies a location feature by providing a structured value representing a feature of an accommodation.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"LocationFeatureSpecification\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the feature.\" },\n        \"value\": { \"type\": \"boolean\", \"description\": \"Whether the feature is available.\"\
  \ }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-place-schema.json
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
title: Schema.org Place
---
