---
name: Clover
x-slug: clover
description: Clover, a First Data company, builds the largest open-architecture point
  of sale solution aimed at small &amp; medium sized business owners. Our products
  are changing the consumer/merchant experience for the better, opening avenues for
  seamless customer-merchant interactions. There are five versions of Clover, including
  the Clover Station, Clover Mobile, Clover Mini, Clover Go, and Clover Flex. With
  Clover, First Data is aiming to create the largest open architecture operating system
  for commerce-enabling solutions and applications for business owners.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
x-kinRank: "7"
x-alexaRank: "23096"
tags: Modifications
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/apis.md
specificationVersion: "0.14"
apis:
- name: ' - Apply a modification to a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodifications-post
  description: 'Create a modification, a record of a modifier as it exists at the
    time it is applied to the lineItem. To view current modifications use an ''expand=modifications''
    query parameter on the lineItem. To learn more about applying a modification see:
    https://docs.clover.com/build/working-with-orders/#add-item-modifiers'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodifications-post-openapi.md
- name: ' - Remove a modification from a line item'
  x-api-slug: v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete
  description: Delete a modification by UUID, removing the record of an applied modification
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidordersorderidline-itemslineitemidmodificationsmodificationid-delete-openapi.md
- name: ' - Get a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-get
  description: Get a single modifier group by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-get-openapi.md
- name: ' - Update a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-post
  description: Update a modifier group. In order to add modifiers use the create modifiers
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-post-openapi.md
- name: ' - Delete a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
  description: Delete an existing modifier group, identified by UUID. This also deletes
    all modifiers within that group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-delete-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Get all modifier groups'
  x-api-slug: v3merchantsmidmodifier-groups-get
  description: These groupings are the categories different modifiers belong to. Modifier
    groups can be made available for specific inventory Items by creating an item
    to modifier group association.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groups-get-openapi.md
- name: ' - Create a modifier group'
  x-api-slug: v3merchantsmidmodifier-groups-post
  description: Create a new modifier group. Modifiers can be associated with a modifier
    group after it has been created.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groups-post-openapi.md
- name: ' - Get a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-get
  description: Get a single modifier group by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-get-openapi.md
- name: ' - Update a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-post
  description: Update a modifier group. In order to add modifiers use the create modifiers
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-post-openapi.md
- name: ' - Delete a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
  description: Delete an existing modifier group, identified by UUID. This also deletes
    all modifiers within that group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-delete-openapi.md
- name: ' - Create or delete item to modifier group associations'
  x-api-slug: v3merchantsmiditem-modifier-groups-post
  description: 'Create or delete one or more association objects (item modifier groups).
    Modifiers can only be applied to items associated with that modifier''s group.
    Learn more about object associations here: https://docs.clover.com/build/web-api/#object-associations'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmiditem-modifier-groups-post-openapi.md
- name: ' - Update the priorities for a collection of up to 200 modifier groups at
    a time'
  x-api-slug: v3merchantsmidmodifier-group-sort-orders-post
  description: Update the priorities for a collection of up to 200 modifier groups
    at a time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-group-sort-orders-post-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Get all modifiers'
  x-api-slug: v3merchantsmidmodifiers-get
  description: Get all modifiers regardless of their modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifiers-get-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Get a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-get
  description: Get a single modifier group by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-get-openapi.md
- name: ' - Update a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-post
  description: Update a modifier group. In order to add modifiers use the create modifiers
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-post-openapi.md
- name: ' - Delete a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
  description: Delete an existing modifier group, identified by UUID. This also deletes
    all modifiers within that group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-delete-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Get all modifier groups'
  x-api-slug: v3merchantsmidmodifier-groups-get
  description: These groupings are the categories different modifiers belong to. Modifier
    groups can be made available for specific inventory Items by creating an item
    to modifier group association.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groups-get-openapi.md
- name: ' - Create a modifier group'
  x-api-slug: v3merchantsmidmodifier-groups-post
  description: Create a new modifier group. Modifiers can be associated with a modifier
    group after it has been created.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groups-post-openapi.md
- name: ' - Get a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-get
  description: Get a single modifier group by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-get-openapi.md
- name: ' - Update a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-post
  description: Update a modifier group. In order to add modifiers use the create modifiers
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-post-openapi.md
- name: ' - Delete a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
  description: Delete an existing modifier group, identified by UUID. This also deletes
    all modifiers within that group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-delete-openapi.md
- name: ' - Create or delete item to modifier group associations'
  x-api-slug: v3merchantsmiditem-modifier-groups-post
  description: 'Create or delete one or more association objects (item modifier groups).
    Modifiers can only be applied to items associated with that modifier''s group.
    Learn more about object associations here: https://docs.clover.com/build/web-api/#object-associations'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmiditem-modifier-groups-post-openapi.md
- name: ' - Update the priorities for a collection of up to 200 modifier groups at
    a time'
  x-api-slug: v3merchantsmidmodifier-group-sort-orders-post
  description: Update the priorities for a collection of up to 200 modifier groups
    at a time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-group-sort-orders-post-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Get all modifiers'
  x-api-slug: v3merchantsmidmodifiers-get
  description: Get all modifiers regardless of their modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifiers-get-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Delete a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
  description: Delete an existing modifier group, identified by UUID. This also deletes
    all modifiers within that group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-delete-openapi.md
- name: ' - Update a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-post
  description: Update a modifier group. In order to add modifiers use the create modifiers
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-post-openapi.md
- name: ' - Get a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-get
  description: Get a single modifier group by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-get-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Update the priorities for a collection of up to 200 modifier groups at
    a time'
  x-api-slug: v3merchantsmidmodifier-group-sort-orders-post
  description: Update the priorities for a collection of up to 200 modifier groups
    at a time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-group-sort-orders-post-openapi.md
- name: ' - Create or delete item to modifier group associations'
  x-api-slug: v3merchantsmiditem-modifier-groups-post
  description: 'Create or delete one or more association objects (item modifier groups).
    Modifiers can only be applied to items associated with that modifier''s group.
    Learn more about object associations here: https://docs.clover.com/build/web-api/#object-associations'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmiditem-modifier-groups-post-openapi.md
- name: ' - Delete a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-delete
  description: Delete an existing modifier group, identified by UUID. This also deletes
    all modifiers within that group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-delete-openapi.md
- name: ' - Update a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-post
  description: Update a modifier group. In order to add modifiers use the create modifiers
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-post-openapi.md
- name: ' - Get a modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupid-get
  description: Get a single modifier group by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupid-get-openapi.md
- name: ' - Create a modifier group'
  x-api-slug: v3merchantsmidmodifier-groups-post
  description: Create a new modifier group. Modifiers can be associated with a modifier
    group after it has been created.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groups-post-openapi.md
- name: ' - Get all modifier groups'
  x-api-slug: v3merchantsmidmodifier-groups-get
  description: These groupings are the categories different modifiers belong to. Modifier
    groups can be made available for specific inventory Items by creating an item
    to modifier group association.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groups-get-openapi.md
- name: ' - Delete a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete
  description: Delete a single modifier by it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-delete-openapi.md
- name: ' - Update a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post
  description: Update a modifier. Note that once it has been created, it is not possible
    to change a modifier's group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-post-openapi.md
- name: ' - Get a single modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get
  description: Get a single modifier by it's group, and it's UUID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiersmodid-get-openapi.md
- name: ' - Create a modifier'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-post
  description: Create a modifier object belonging to the modifier group identified
    in the URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-post-openapi.md
- name: ' - Get all modifiers belonging to a single modifier group'
  x-api-slug: v3merchantsmidmodifier-groupsmodgroupidmodifiers-get
  description: Get an array containing the modifiers in a single modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifier-groupsmodgroupidmodifiers-get-openapi.md
- name: ' - Get all modifiers'
  x-api-slug: v3merchantsmidmodifiers-get
  description: Get all modifiers regardless of their modifier group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/clover-logo.png
  humanURL: https://www.clover.com
  baseURL: https:///merchants/https://api.clover.com
  tags: SaaS, Technology, Mobile, internet, Point of Sale, Pos, Service API, Relative
    Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/modifications/master/_listings/clover/v3merchantsmidmodifiers-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://cloudflare.api.gallery.streamdata.io
- type: x-api-stack
  url: http://clover.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/clover
- type: x-developer
  url: https://www.clover.com/developers
- type: x-documentation
  url: https://docs.clover.com/
- type: x-github
  url: https://github.com/clover
- type: x-twitter
  url: https://twitter.com/CloverPOS
- type: x-website
  url: https://www.clover.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---