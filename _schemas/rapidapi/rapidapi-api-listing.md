---
description: Schema representing an API listing on the RapidAPI platform, including metadata, versioning, endpoint definitions, and pricing plans.
layout: schema
name: RapidAPI API Listing
properties_list:
- description: Unique identifier for the API listing on the platform
  name: id
  type: string
- description: Display name of the API as shown on the marketplace
  name: name
  type: string
- description: URL-friendly slug used in the API's marketplace URL
  name: slug
  type: string
- description: Short description of the API displayed on the endpoints tab
  name: description
  type: string
- description: Detailed description with use cases and documentation, displayed on the about tab
  name: longDescription
  type: string
- description: The category the API is listed under for organization and discovery
  name: category
  type: string
- description: Custom tags applied to the API for filtering and search
  name: tags
  type: array
- description: URL to the website providing the API, shown on the about tab
  name: websiteUrl
  type: string
- description: URL to the API icon image, recommended 500x500 px in PNG or JPG format
  name: imageUrl
  type: string
- description: Current publication status of the API listing
  name: status
  type: string
- description: Whether the API provider has been verified by RapidAPI
  name: isVerified
  type: boolean
- description: Information about the organization or user providing the API
  name: provider
  type: object
- description: Available versions of the API
  name: versions
  type: array
- description: Endpoint definitions for the current active version
  name: endpoints
  type: array
- description: Subscription pricing plans available for this API
  name: plans
  type: array
- description: Average user rating on a scale of 0 to 5
  name: averageRating
  type: number
- description: Total number of user ratings
  name: totalRatings
  type: integer
- description: Timestamp when the API listing was first created
  name: createdAt
  type: string
- description: Timestamp when the API listing was last modified
  name: updatedAt
  type: string
provider_name: RapidAPI
provider_slug: rapidapi
schema_file: json-schema/rapidapi-api-listing-schema.json
slug: rapidapi-api-listing
source_filename: rapidapi-api-listing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rapidapi.com/schemas/rapidapi/api-listing.json\",\n  \"title\": \"RapidAPI API Listing\",\n  \"description\": \"Schema representing an API listing on the RapidAPI platform, including metadata, versioning, endpoint definitions, and pricing plans.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"description\", \"category\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API listing on the platform\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the API as shown on the marketplace\",\n      \"minLength\": 1,\n      \"maxLength\": 200\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly slug used in the API's marketplace URL\",\n      \"pattern\": \"^[a-z0-9-]+$\"\n    },\n    \"description\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Short description of the API displayed on the endpoints tab\",\n      \"maxLength\": 500\n    },\n    \"longDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description with use cases and documentation, displayed on the about tab\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category the API is listed under for organization and discovery\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Custom tags applied to the API for filtering and search\"\n    },\n    \"websiteUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the website providing the API, shown on the about tab\"\n    },\n    \"imageUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the API icon image, recommended 500x500 px in PNG or JPG format\"\
  \n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"deprecated\"],\n      \"description\": \"Current publication status of the API listing\"\n    },\n    \"isVerified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the API provider has been verified by RapidAPI\"\n    },\n    \"provider\": {\n      \"$ref\": \"#/$defs/Provider\",\n      \"description\": \"Information about the organization or user providing the API\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ApiVersion\"\n      },\n      \"description\": \"Available versions of the API\"\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ApiEndpoint\"\n      },\n      \"description\": \"Endpoint definitions for the current active version\"\n    },\n    \"plans\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PricingPlan\"\
  \n      },\n      \"description\": \"Subscription pricing plans available for this API\"\n    },\n    \"averageRating\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"minimum\": 0,\n      \"maximum\": 5,\n      \"description\": \"Average user rating on a scale of 0 to 5\"\n    },\n    \"totalRatings\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total number of user ratings\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API listing was first created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API listing was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"Provider\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the API provider\"\
  \n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the API provider\"\n        },\n        \"organizationId\": {\n          \"type\": \"string\",\n          \"description\": \"Organization the provider belongs to, if applicable\"\n        },\n        \"isVerified\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the provider has been verified\"\n        }\n      },\n      \"description\": \"Information about an API provider on the platform\"\n    },\n    \"ApiVersion\": {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the version\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Version name or label\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"deprecated\"\
  , \"draft\"],\n          \"description\": \"Current status of the version\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the version was created\"\n        }\n      },\n      \"description\": \"A version of an API listing\"\n    },\n    \"ApiEndpoint\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"method\", \"path\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the endpoint\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the endpoint\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"],\n          \"description\": \"HTTP method for the endpoint\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n         \
  \ \"description\": \"URL path for the endpoint\"\n        },\n        \"group\": {\n          \"type\": \"string\",\n          \"description\": \"Endpoint group for organizational purposes\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of what the endpoint does\"\n        },\n        \"parameters\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/EndpointParameter\"\n          },\n          \"description\": \"Parameters accepted by this endpoint\"\n        }\n      },\n      \"description\": \"An individual endpoint within an API\"\n    },\n    \"EndpointParameter\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"location\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Parameter name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Data type of\
  \ the parameter\"\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the parameter is required\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the parameter\"\n        },\n        \"defaultValue\": {\n          \"type\": \"string\",\n          \"description\": \"Default value if not provided\"\n        },\n        \"location\": {\n          \"type\": \"string\",\n          \"enum\": [\"query\", \"path\", \"header\", \"body\"],\n          \"description\": \"Where the parameter is sent in the request\"\n        }\n      },\n      \"description\": \"A parameter accepted by an API endpoint\"\n    },\n    \"PricingPlan\": {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the plan\"\n        },\n        \"name\": {\n      \
  \    \"type\": \"string\",\n          \"description\": \"Plan name such as Basic, Pro, or Ultra\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": 0,\n          \"description\": \"Monthly price in USD, 0 for free tier\"\n        },\n        \"rateLimit\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Maximum number of requests allowed per month\"\n        },\n        \"quotaType\": {\n          \"type\": \"string\",\n          \"enum\": [\"hard\", \"soft\"],\n          \"description\": \"Whether exceeding the limit blocks requests or incurs overage charges\"\n        },\n        \"features\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Features included in this plan\"\n        }\n      },\n      \"description\": \"A subscription pricing plan for an API\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/json-schema/rapidapi-api-listing-schema.json
tags:
- API Marketplace
- API Management
- API Testing
- API Gateway
- API Design
- Enterprise
title: RapidAPI API Listing
---
