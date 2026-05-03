---
description: A particular physical business or branch of an organization. Examples of LocalBusiness include a restaurant, a particular branch of a restaurant chain, a bank branch, a medical practice, a club, a bowling alley, etc.
layout: schema
name: Schema.org LocalBusiness
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the business.
  name: name
  type: string
- description: A description of the business.
  name: description
  type: string
- description: URL of the business.
  name: url
  type: string
- description: An image of the business.
  name: image
  type: object
- description: An associated logo.
  name: logo
  type: object
- description: Physical address of the business.
  name: address
  type: object
- description: The geo coordinates of the business.
  name: geo
  type: object
- description: The telephone number.
  name: telephone
  type: string
- description: Email address.
  name: email
  type: string
- description: The fax number.
  name: faxNumber
  type: string
- description: The general opening hours for a business (e.g., Mo-Fr 08:00-17:00).
  name: openingHours
  type: object
- description: The opening hours of a certain place.
  name: openingHoursSpecification
  type: object
- description: The price range of the business (e.g., $$$).
  name: priceRange
  type: string
- description: The currency accepted.
  name: currenciesAccepted
  type: string
- description: Cash, Credit Card, Cryptocurrency, Local Exchange Tradings System, etc.
  name: paymentAccepted
  type: string
- description: The geographic area where a service or offered item is provided.
  name: areaServed
  type: string
- description: A URL to a map of the place.
  name: hasMap
  type: string
- description: The overall rating.
  name: aggregateRating
  type: object
- description: A review of the business.
  name: review
  type: object
- description: A department within the business.
  name: department
  type: object
- description: A person who founded this business.
  name: founder
  type: object
- description: The date that this business was founded.
  name: foundingDate
  type: string
- description: URL of the menu (for FoodEstablishment).
  name: menu
  type: string
- description: The cuisine of the restaurant (for FoodEstablishment).
  name: servesCuisine
  type: string
- description: Indicates whether a FoodEstablishment accepts reservations.
  name: acceptsReservations
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
- description: The identifier property represents any kind of identifier.
  name: identifier
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-local-business-schema.json
slug: schema-org-local-business
source_filename: schema-org-local-business-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/local-business.json\",\n  \"title\": \"Schema.org LocalBusiness\",\n  \"description\": \"A particular physical business or branch of an organization. Examples of LocalBusiness include a restaurant, a particular branch of a restaurant chain, a bank branch, a medical practice, a club, a bowling alley, etc.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"LocalBusiness\", \"AnimalShelter\", \"AutomotiveBusiness\", \"ChildCare\", \"Dentist\", \"DryCleaningOrLaundry\", \"EmergencyService\", \"EmploymentAgency\", \"EntertainmentBusiness\", \"FinancialService\", \"FoodEstablishment\", \"GovernmentOffice\", \"HealthAndBeautyBusiness\", \"HomeAndConstructionBusiness\", \"InternetCafe\", \"LegalService\", \"Library\", \"LodgingBusiness\"\
  , \"MedicalBusiness\", \"ProfessionalService\", \"RadioStation\", \"RealEstateAgent\", \"RecyclingCenter\", \"SelfStorage\", \"ShoppingCenter\", \"SportsActivityLocation\", \"Store\", \"TelevisionStation\", \"TouristInformationCenter\", \"TravelAgency\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the business.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the business.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the business.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the business.\"\n    },\n    \"logo\": {\n      \"oneOf\": [\n        { \"\
  type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An associated logo.\"\n    },\n    \"address\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"schema-org-postal-address-schema.json\" }\n      ],\n      \"description\": \"Physical address of the business.\"\n    },\n    \"geo\": {\n      \"$ref\": \"schema-org-geo-coordinates-schema.json\",\n      \"description\": \"The geo coordinates of the business.\"\n    },\n    \"telephone\": {\n      \"type\": \"string\",\n      \"description\": \"The telephone number.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address.\"\n    },\n    \"faxNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The fax number.\"\n    },\n    \"openingHours\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\"\
  : { \"type\": \"string\" } }\n      ],\n      \"description\": \"The general opening hours for a business (e.g., Mo-Fr 08:00-17:00).\"\n    },\n    \"openingHoursSpecification\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/OpeningHoursSpecification\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/OpeningHoursSpecification\" } }\n      ],\n      \"description\": \"The opening hours of a certain place.\"\n    },\n    \"priceRange\": {\n      \"type\": \"string\",\n      \"description\": \"The price range of the business (e.g., $$$).\"\n    },\n    \"currenciesAccepted\": {\n      \"type\": \"string\",\n      \"description\": \"The currency accepted.\"\n    },\n    \"paymentAccepted\": {\n      \"type\": \"string\",\n      \"description\": \"Cash, Credit Card, Cryptocurrency, Local Exchange Tradings System, etc.\"\n    },\n    \"areaServed\": {\n      \"type\": \"string\",\n      \"description\": \"The geographic area where a service or offered item is provided.\"\
  \n    },\n    \"hasMap\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to a map of the place.\"\n    },\n    \"aggregateRating\": {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A review of the business.\"\n    },\n    \"department\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"A department within the business.\"\n    },\n    \"founder\": {\n      \"$ref\": \"schema-org-person-schema.json\",\n      \"description\": \"A person who founded this business.\"\n    },\n    \"foundingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\
  ,\n      \"description\": \"The date that this business was founded.\"\n    },\n    \"menu\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the menu (for FoodEstablishment).\"\n    },\n    \"servesCuisine\": {\n      \"type\": \"string\",\n      \"description\": \"The cuisine of the restaurant (for FoodEstablishment).\"\n    },\n    \"acceptsReservations\": {\n      \"oneOf\": [\n        { \"type\": \"boolean\" },\n        { \"type\": \"string\", \"format\": \"uri\" }\n      ],\n      \"description\": \"Indicates whether a FoodEstablishment accepts reservations.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The identifier property represents any kind of identifier.\"\n    }\n  },\n  \"$defs\": {\n    \"OpeningHoursSpecification\": {\n      \"type\": \"object\",\n      \"description\": \"A structured value providing information about the opening hours of a place.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"OpeningHoursSpecification\" },\n        \"dayOfWeek\": { \"type\": \"string\", \"enum\": [\"Monday\", \"Tuesday\", \"Wednesday\", \"Thursday\", \"Friday\", \"Saturday\", \"Sunday\", \"PublicHolidays\"] },\n        \"opens\": { \"type\": \"string\", \"pattern\": \"^\\\\d{2}:\\\\d{2}$\" },\n        \"closes\": { \"type\": \"string\", \"pattern\": \"^\\\\d{2}:\\\\d{2}$\" },\n        \"validFrom\": { \"type\": \"string\", \"format\": \"date\" },\n        \"validThrough\": { \"type\": \"string\", \"format\": \"date\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-local-business-schema.json
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
title: Schema.org LocalBusiness
---
