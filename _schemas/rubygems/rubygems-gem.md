---
description: A Ruby gem hosted on RubyGems.org, representing a packaged Ruby library or application distributed through the RubyGems package registry.
layout: schema
name: RubyGems Gem
properties_list:
- description: The unique name of the gem on RubyGems.org
  name: name
  type: string
- description: Total number of downloads across all versions of this gem
  name: downloads
  type: integer
- description: The current (latest) version number following Ruby versioning conventions
  name: version
  type: string
- description: ISO 8601 timestamp when the current version was published
  name: version_created_at
  type: string
- description: Number of downloads for the current version
  name: version_downloads
  type: integer
- description: The platform the gem targets (e.g., ruby, java, x86_64-linux)
  name: platform
  type: string
- description: Comma-separated list of gem authors
  name: authors
  type: string
- description: Short description of the gem
  name: info
  type: string
- description: SPDX license identifiers for the gem
  name: licenses
  type: array
- description: Additional metadata key-value pairs defined in the gemspec
  name: metadata
  type: object
- description: Whether the current version has been yanked from the registry
  name: yanked
  type: boolean
- description: SHA-256 checksum of the gem file
  name: sha
  type: string
- description: URI to the gem project page on RubyGems.org
  name: project_uri
  type: string
- description: URI to download the gem file
  name: gem_uri
  type: string
- description: URI to the gem homepage
  name: homepage_uri
  type:
  - string
  - 'null'
- description: URI to the gem wiki
  name: wiki_uri
  type:
  - string
  - 'null'
- description: URI to the gem documentation
  name: documentation_uri
  type:
  - string
  - 'null'
- description: URI to the gem mailing list
  name: mailing_list_uri
  type:
  - string
  - 'null'
- description: URI to the gem source code repository
  name: source_code_uri
  type:
  - string
  - 'null'
- description: URI to the gem bug tracker
  name: bug_tracker_uri
  type:
  - string
  - 'null'
- description: URI to the gem changelog
  name: changelog_uri
  type:
  - string
  - 'null'
- description: URI to the gem funding page
  name: funding_uri
  type:
  - string
  - 'null'
- description: ''
  name: dependencies
  type: object
provider_name: RubyGems
provider_slug: rubygems
schema_file: json-schema/rubygems-gem-schema.json
slug: rubygems-gem
source_filename: rubygems-gem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rubygems.org/schemas/rubygems/gem.json\",\n  \"title\": \"RubyGems Gem\",\n  \"description\": \"A Ruby gem hosted on RubyGems.org, representing a packaged Ruby library or application distributed through the RubyGems package registry.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"version\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the gem on RubyGems.org\",\n      \"pattern\": \"^[a-zA-Z0-9._-]+$\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"downloads\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of downloads across all versions of this gem\",\n      \"minimum\": 0\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The current (latest) version number following Ruby versioning conventions\",\n      \"pattern\": \"^[0-9]+(\\\
  \\.[0-9]+)*(\\\\.[a-zA-Z0-9]+)*$\"\n    },\n    \"version_created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the current version was published\"\n    },\n    \"version_downloads\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of downloads for the current version\",\n      \"minimum\": 0\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform the gem targets (e.g., ruby, java, x86_64-linux)\",\n      \"default\": \"ruby\"\n    },\n    \"authors\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of gem authors\"\n    },\n    \"info\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the gem\"\n    },\n    \"licenses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"SPDX license identifiers for the gem\"\n    },\n    \"metadata\"\
  : {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional metadata key-value pairs defined in the gemspec\"\n    },\n    \"yanked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current version has been yanked from the registry\"\n    },\n    \"sha\": {\n      \"type\": \"string\",\n      \"description\": \"SHA-256 checksum of the gem file\",\n      \"pattern\": \"^[a-f0-9]{64}$\"\n    },\n    \"project_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URI to the gem project page on RubyGems.org\"\n    },\n    \"gem_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URI to download the gem file\"\n    },\n    \"homepage_uri\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URI to the gem homepage\"\n    },\n    \"wiki_uri\": {\n      \"type\": [\"\
  string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URI to the gem wiki\"\n    },\n    \"documentation_uri\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URI to the gem documentation\"\n    },\n    \"mailing_list_uri\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URI to the gem mailing list\"\n    },\n    \"source_code_uri\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URI to the gem source code repository\"\n    },\n    \"bug_tracker_uri\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URI to the gem bug tracker\"\n    },\n    \"changelog_uri\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URI to the gem changelog\"\n    },\n    \"funding_uri\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\"\
  : \"uri\",\n      \"description\": \"URI to the gem funding page\"\n    },\n    \"dependencies\": {\n      \"$ref\": \"#/$defs/Dependencies\"\n    }\n  },\n  \"$defs\": {\n    \"Dependencies\": {\n      \"type\": \"object\",\n      \"description\": \"Runtime and development dependency lists for the gem\",\n      \"properties\": {\n        \"development\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Dependency\"\n          },\n          \"description\": \"Dependencies needed only during development\"\n        },\n        \"runtime\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Dependency\"\n          },\n          \"description\": \"Dependencies required at runtime\"\n        }\n      }\n    },\n    \"Dependency\": {\n      \"type\": \"object\",\n      \"description\": \"A dependency on another gem with version constraints\",\n      \"required\": [\"name\", \"requirements\"],\n      \"properties\"\
  : {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the dependency gem\"\n        },\n        \"requirements\": {\n          \"type\": \"string\",\n          \"description\": \"Version requirement string (e.g., '>= 1.0', '~> 2.0')\"\n        }\n      }\n    },\n    \"GemVersion\": {\n      \"type\": \"object\",\n      \"description\": \"A specific version of a Ruby gem with build and publication metadata\",\n      \"required\": [\"number\"],\n      \"properties\": {\n        \"authors\": {\n          \"type\": \"string\",\n          \"description\": \"Comma-separated list of version authors\"\n        },\n        \"built_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the version was built\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the version\
  \ was published\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Full description of the gem version\"\n        },\n        \"downloads_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of downloads for this version\",\n          \"minimum\": 0\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Additional metadata for this version\"\n        },\n        \"number\": {\n          \"type\": \"string\",\n          \"description\": \"The version number\"\n        },\n        \"summary\": {\n          \"type\": \"string\",\n          \"description\": \"Short summary of the gem version\"\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"The platform for this version\"\n        },\n        \"rubygems_version\": {\n         \
  \ \"type\": \"string\",\n          \"description\": \"Minimum RubyGems version required\"\n        },\n        \"ruby_version\": {\n          \"type\": \"string\",\n          \"description\": \"Minimum Ruby version required\"\n        },\n        \"prerelease\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a prerelease version\"\n        },\n        \"licenses\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"SPDX license identifiers for this version\"\n        },\n        \"requirements\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"System requirements for this version\"\n        },\n        \"sha\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-256 checksum of the gem file\",\n          \"pattern\": \"^[a-f0-9]{64}$\"\n        }\n      }\n    },\n\
  \    \"Owner\": {\n      \"type\": \"object\",\n      \"description\": \"A gem owner on RubyGems.org\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique user ID\"\n        },\n        \"handle\": {\n          \"type\": \"string\",\n          \"description\": \"User handle on RubyGems.org\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"User email address\"\n        }\n      }\n    },\n    \"Webhook\": {\n      \"type\": \"object\",\n      \"description\": \"A webhook subscription on RubyGems.org\",\n      \"required\": [\"url\"],\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL that receives webhook POST notifications\"\n        },\n        \"failure_count\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Number of consecutive delivery failures\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rubygems/refs/heads/main/json-schema/rubygems-gem-schema.json
tags:
- Ruby
- Package Manager
- Open Source
- Developer Tools
title: RubyGems Gem
---
