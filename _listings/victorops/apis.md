---
name: VictorOps
x-slug: victorops
description: VictorOps incident managament software gives DevOps observability, collaboration,
  & real-time alerting, to build, deploy, & operate software. Learn more.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
x-kinRank: "8"
x-alexaRank: "196587"
tags: VictorOps
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apis.md
specificationVersion: "0.14"
apis:
- name: Victor Ops Retrieve alert details.
  x-api-slug: victor-ops
  description: |-
    Retrieve the details of an alert that was sent VictorOps by you.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/alerts/{uuid}
  tags: Alerts,Uuid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1alertsuuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1alertsuuid-get-openapi.md
- name: Victor Ops Get current incident information
  x-api-slug: victor-ops
  description: |-
    Get a list of the currently open, acknowledged and recently resolved incidents.
    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidents-get-openapi.md
- name: Victor Ops Create a new incident
  x-api-slug: victor-ops
  description: |-
    Create a new incident.

    This call replicates the function of our
    manual incident creation process.
    Monitoring tools and custom integrations
    should be configured using our
    REST Endpoint.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents
  tags: Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidents-post-openapi.md
- name: Victor Ops Acknowledge an incident or list of incidents
  x-api-slug: victor-ops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/ack
  tags: Incidents,Ack
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsack-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsack-patch-openapi.md
- name: Victor Ops Acknowledge all incidents for which a user was paged.
  x-api-slug: victor-ops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/byUser/ack
  tags: Incidents,ByUser,Ack
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsbyuserack-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsbyuserack-patch-openapi.md
- name: Victor Ops Resolve all incidents for which a user was paged.
  x-api-slug: victor-ops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/byUser/resolve
  tags: Incidents,ByUser,Resolve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsbyuserresolve-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsbyuserresolve-patch-openapi.md
- name: Victor Ops Reroute one or more incidents to one or more new routable destinations.
  x-api-slug: victor-ops
  description: Reroute one or more incidents to one or more users and/or escalation
    policies
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/reroute
  tags: Incidents,Reroute
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsreroute-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsreroute-post-openapi.md
- name: Victor Ops Resolve an incident or list of incidents
  x-api-slug: victor-ops
  description: |-
    The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/incidents/resolve
  tags: Incidents,Resolve
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsresolve-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1incidentsresolve-patch-openapi.md
- name: Victor Ops Get an organization's on-call users
  x-api-slug: victor-ops
  description: |-
    Get all on-call uesrs/teams for your organization.

    This API may be called a maximum of 1 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/oncall/current
  tags: Oncall,Current
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1oncallcurrent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1oncallcurrent-get-openapi.md
- name: Victor Ops List routing keys with associated teams
  x-api-slug: victor-ops
  description: |-
    Retrieves a list of routing keys and associated teams.
    This API may be called a maximum of once a minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/org/routing-keys
  tags: Org,Routing-keys
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1orgroutingkeys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1orgroutingkeys-get-openapi.md
- name: Victor Ops Get escalation policy info
  x-api-slug: victor-ops
  description: |-
    Retrieves a list of escalation policy information.
    This API may be called a maximum of once a minute
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/policies
  tags: Policies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policies-get-openapi.md
- name: Victor Ops Get the available contact types
  x-api-slug: victor-ops
  description: |-
    Get the available contact types

    description: "Email Address", type: "email"
    description: "Phone Number", type: "phone"

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/policies/types/contacts
  tags: Policies,Types,Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policiestypescontacts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policiestypescontacts-get-openapi.md
- name: Victor Ops Get the available notification types
  x-api-slug: victor-ops
  description: |-
    Get the available notification types

    description: "Send a push notification to all my devices", type: "push"
    description: "Send an email to an email address", type: "email"
    description: "Send an SMS to a phone number", type: "sms"
    description: "Make a phone call to a phone number", type: "phone"

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/policies/types/notifications
  tags: Policies,Types,Notifications
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policiestypesnotifications-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policiestypesnotifications-get-openapi.md
- name: Victor Ops Get the available timeout values
  x-api-slug: victor-ops
  description: |-
    Get the available timeout values

    description: "If still unacked after 1 minute", type: 1
    description: "If still unacked after 5 minutes", type: 5
    description: "If still unacked after 10 minutes", type: 10
    description: "If still unacked after 15 minutes", type: 15
    description: "If still unacked after 20 minutes", type: 20
    description: "If still unacked after 25 minutes", type: 25
    description: "If still unacked after 30 minutes", type: 30
    description: "If still unacked after 45 minutes", type: 45
    description: "If still unacked after 60 minutes", type: 60

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/policies/types/timeouts
  tags: Policies,Types,Timeouts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policiestypestimeouts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policiestypestimeouts-get-openapi.md
- name: Victor Ops Create an on-call override (take on-call)
  x-api-slug: victor-ops
  description: |-
    Replaces a currently on-call user in the escalation policy with another.  In many cases, the policy slug
    will match the slug of the team that contains it.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/policies/{policy}/oncall/user
  tags: Policies,Policy,Oncall,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policiespolicyoncalluser-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1policiespolicyoncalluser-patch-openapi.md
- name: Victor Ops Get the user's paging policy
  x-api-slug: victor-ops
  description: |-
    Get all the paging policy steps for the user on the org associated with the API key

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/profile/{username}/policies
  tags: Profile,Username,Policies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepolicies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepolicies-get-openapi.md
- name: Victor Ops Create a paging policy step
  x-api-slug: victor-ops
  description: |-
    Create a paging policy step

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/profile/{username}/policies
  tags: Profile,Username,Policies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepolicies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepolicies-post-openapi.md
- name: Victor Ops Get a paging policy step
  x-api-slug: victor-ops
  description: |-
    Get a paging policy step

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/profile/{username}/policies/{step}
  tags: Profile,Username,Policies,Step
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciesstep-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciesstep-get-openapi.md
- name: Victor Ops Create a rule for a paging policy step
  x-api-slug: victor-ops
  description: |-
    Create a rule for a paging policy step

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/profile/{username}/policies/{step}
  tags: Profile,Username,Policies,Step
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciesstep-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciesstep-post-openapi.md
- name: Victor Ops Update a paging policy step
  x-api-slug: victor-ops
  description: |-
    Update a paging policy step

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/profile/{username}/policies/{step}
  tags: Profile,Username,Policies,Step
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciesstep-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciesstep-put-openapi.md
- name: Victor Ops Delete a rule from a paging policy step
  x-api-slug: victor-ops
  description: |-
    Delete a rule from a paging policy step

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/profile/{username}/policies/{step}/{rule}
  tags: Profile,Username,Policies,Step,Rule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciessteprule-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciessteprule-delete-openapi.md
- name: Victor Ops Get a rule from a paging policy step
  x-api-slug: victor-ops
  description: |-
    Get a rule from a paging policy step

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/profile/{username}/policies/{step}/{rule}
  tags: Profile,Username,Policies,Step,Rule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciessteprule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciessteprule-get-openapi.md
- name: Victor Ops Update a rule for a paging policy step
  x-api-slug: victor-ops
  description: |-
    Update a rule for a paging policy step

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/profile/{username}/policies/{step}/{rule}
  tags: Profile,Username,Policies,Step,Rule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciessteprule-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1profileusernamepoliciessteprule-put-openapi.md
- name: Victor Ops List teams
  x-api-slug: victor-ops
  description: |-
    Get a list of teams for your organization.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team
  tags: Team
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1team-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1team-get-openapi.md
- name: Victor Ops Add a team
  x-api-slug: victor-ops
  description: |-
    Add a team to your organization.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team
  tags: Team
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1team-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1team-post-openapi.md
- name: Victor Ops Remove a team
  x-api-slug: victor-ops
  description: |-
    Remove a team from your organization.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}
  tags: Team,Team
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteam-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteam-delete-openapi.md
- name: Victor Ops Retrieve information for a team
  x-api-slug: victor-ops
  description: |-
    Get the information for the specified team.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}
  tags: Team,Team
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteam-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteam-get-openapi.md
- name: Victor Ops Update a team
  x-api-slug: victor-ops
  description: |-
    Update the designated team

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}
  tags: Team,Team
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteam-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteam-put-openapi.md
- name: Victor Ops Retrieve a list of members for a team
  x-api-slug: victor-ops
  description: |-
    Get the members for the specified team.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}/members
  tags: Team,Team,Members
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteammembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteammembers-get-openapi.md
- name: Victor Ops Add a team member
  x-api-slug: victor-ops
  description: |-
    Add a team member to your team.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}/members
  tags: Team,Team,Members
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteammembers-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteammembers-post-openapi.md
- name: Victor Ops Remove a team member
  x-api-slug: victor-ops
  description: |-
    Remove a team from your organization.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}/members/{user}
  tags: Team,Team,Members,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteammembersuser-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteammembersuser-delete-openapi.md
- name: Victor Ops Get a team's on-call schedule
  x-api-slug: victor-ops
  description: |-
    __NOTE: This call is deprecated. Please use `GET /api-public/v2/team/{team}/oncall/schedule`.__

    Get the on-call schedule for a team, including on-call overrides.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}/oncall/schedule
  tags: Team,Team,Oncall,Schedule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteamoncallschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteamoncallschedule-get-openapi.md
- name: Victor Ops Create an on-call override (take on-call)
  x-api-slug: victor-ops
  description: |-
    __NOTE: This API call is deprecated. Please use `PATCH /api-public/v2/policies/{policy}/oncall/user`__

    Replaces a currently on-call user on the team with another.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}/oncall/user
  tags: Team,Team,Oncall,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteamoncalluser-patch-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteamoncalluser-patch-openapi.md
- name: Victor Ops Retrieve a list of escalation policies for a team
  x-api-slug: victor-ops
  description: |-
    Get the escalation policies for the specified team.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/team/{team}/policies
  tags: Team,Team,Policies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteampolicies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1teamteampolicies-get-openapi.md
- name: Victor Ops List users
  x-api-slug: victor-ops
  description: |-
    Get a list of users for your organization

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user
  tags: User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1user-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1user-get-openapi.md
- name: Victor Ops Add a user
  x-api-slug: victor-ops
  description: |-
    Add a user to your organization

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user
  tags: User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1user-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1user-post-openapi.md
- name: Victor Ops Remove a user
  x-api-slug: victor-ops
  description: |-
    Remove a user from your organization

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}
  tags: User,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruser-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruser-delete-openapi.md
- name: Victor Ops Retrieve information for a user
  x-api-slug: victor-ops
  description: |-
    Get the information for the specified user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}
  tags: User,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruser-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruser-get-openapi.md
- name: Victor Ops Update a user
  x-api-slug: victor-ops
  description: |-
    Update the designated user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}
  tags: User,User
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruser-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruser-put-openapi.md
- name: Victor Ops Get a list of all contact methods for a user
  x-api-slug: victor-ops
  description: |-
    Get the contact methods for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods
  tags: User,User,Contact-methods
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethods-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethods-get-openapi.md
- name: Victor Ops Get a list of all contact devices for a user
  x-api-slug: victor-ops
  description: |-
    Get the contact methods for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/devices
  tags: User,User,Contact-methods,Devices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsdevices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsdevices-get-openapi.md
- name: Victor Ops Delete a contact device for a user
  x-api-slug: victor-ops
  description: |-
    Delete a contact device for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/devices/{contactId}
  tags: User,User,Contact-methods,Devices,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-delete-openapi.md
- name: Victor Ops Get the indicated contact device for a user
  x-api-slug: victor-ops
  description: |-
    Get the indicated contact device for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/devices/{contactId}
  tags: User,User,Contact-methods,Devices,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-get-openapi.md
- name: Victor Ops Update a contact device for a user
  x-api-slug: victor-ops
  description: |-
    Update a contact device for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/devices/{contactId}
  tags: User,User,Contact-methods,Devices,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsdevicescontactid-put-openapi.md
- name: Victor Ops Get a list of all contact emails for a user
  x-api-slug: victor-ops
  description: |-
    Get the contact emails for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/emails
  tags: User,User,Contact-methods,Emails
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsemails-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsemails-get-openapi.md
- name: Victor Ops Create a contact emails for a user
  x-api-slug: victor-ops
  description: |-
    Create a contact email for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/emails
  tags: User,User,Contact-methods,Emails
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsemails-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsemails-post-openapi.md
- name: Victor Ops Delete a contact email for a user
  x-api-slug: victor-ops
  description: |-
    Delete the indicated contact email for the user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/emails/{contactId}
  tags: User,User,Contact-methods,Emails,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsemailscontactid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsemailscontactid-delete-openapi.md
- name: Victor Ops Get the indicate contact email for a user
  x-api-slug: victor-ops
  description: |-
    Get the indicated contact email for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/emails/{contactId}
  tags: User,User,Contact-methods,Emails,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsemailscontactid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsemailscontactid-get-openapi.md
- name: Victor Ops Get a list of all contact phones for a user
  x-api-slug: victor-ops
  description: |-
    Get the contact phones for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/phones
  tags: User,User,Contact-methods,Phones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsphones-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsphones-get-openapi.md
- name: Victor Ops Create a contact phones for a user
  x-api-slug: victor-ops
  description: |-
    Create a contact phone for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/phones
  tags: User,User,Contact-methods,Phones
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsphones-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsphones-post-openapi.md
- name: Victor Ops Delete a contact phone for a user
  x-api-slug: victor-ops
  description: |-
    Delete the indicated contact phone for the user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/phones/{contactId}
  tags: User,User,Contact-methods,Phones,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsphonescontactid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsphonescontactid-delete-openapi.md
- name: Victor Ops Get the indicate contact phone for a user
  x-api-slug: victor-ops
  description: |-
    Get the indicated contact phone for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/contact-methods/phones/{contactId}
  tags: User,User,Contact-methods,Phones,ContactId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsphonescontactid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1userusercontactmethodsphonescontactid-get-openapi.md
- name: Victor Ops Get a user's on-call schedule
  x-api-slug: victor-ops
  description: |-
    __NOTE: This call is deprecated. Please use `GET /api-public/v2/user/{user}/oncall/schedule`.__

    Get the on-call schedule for a user for all teams, including on-call overrides.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/oncall/schedule
  tags: User,User,Oncall,Schedule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruseroncallschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruseroncallschedule-get-openapi.md
- name: Victor Ops Get a list of paging policies for a user
  x-api-slug: victor-ops
  description: |-
    Get paging policies for a user

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v1/user/{user}/policies
  tags: User,User,Policies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruserpolicies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv1useruserpolicies-get-openapi.md
- name: Victor Ops Get a team's on-call schedule
  x-api-slug: victor-ops
  description: |-
    Get the on-call schedule for a team, including on-call overrides.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v2/team/{team}/oncall/schedule
  tags: Api-public,V2,Team,Team,Oncall,Schedule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv2teamteamoncallschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv2teamteamoncallschedule-get-openapi.md
- name: Victor Ops Get a user's on-call schedule
  x-api-slug: victor-ops
  description: |-
    Get the on-call schedule for a user for all teams the user is on, including on-call overrides.

    This API may be called a maximum of 15 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-public/v2/user/{user}/oncall/schedule
  tags: Api-public,V2,User,User,Oncall,Schedule
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv2useruseroncallschedule-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apipublicv2useruseroncallschedule-get-openapi.md
- name: Victor Ops Get/search incident history
  x-api-slug: victor-ops
  description: |-
    __NOTE: This call is deprecated. Please use `GET /api-reporting/v2/incidents`.__

    Retrieve incident history for your company, searching over date ranges and with filtering options.  This is historical
    data, and may be up to 15 minutes behind real-time incident data.  By default, only resolved incidents will be returned.

    This API may be called a maximum of once a minute.

    Incident requests are paginated with a offset and limit query string parameters.
      The query for incidents is run and offset records are skipped, after which limit records will be returned.

    The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.

    On return, the total number of records available for that query will be returned in the payload as 'total'.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-reporting/v1/incidents
  tags: Api-reporting,V1,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apireportingv1incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apireportingv1incidents-get-openapi.md
- name: Victor Ops A list of shift changes for a team
  x-api-slug: victor-ops
  description: |-
    Returns a log of user shift changes for the specified team. This is historical
    data, and may be up to 15 minutes behind real-time log data.

    This API may be called a maximum of 6 times per minute.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-reporting/v1/team/{team}/oncall/log
  tags: Api-reporting,V1,Team,Team,Oncall,Log
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apireportingv1teamteamoncalllog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apireportingv1teamteamoncalllog-get-openapi.md
- name: Victor Ops Get/search incident history
  x-api-slug: victor-ops
  description: |-
    Retrieve incident history for your company, searching over date ranges and with filtering options.

    This API may be called a maximum of once a minute.

    Incident requests are paginated with a offset and limit query string parameters.
      The query for incidents is run and offset records are skipped, after which limit records will be returned.

    The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.

    Unless specified otherwise with the parameter currentPhase, the response will only contain resolved incidents.

    On return, the total number of records available for that query will be returned in the payload as 'total'.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com////api-reporting/v2/incidents
  tags: Api-reporting,V2,Incidents
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apireportingv2incidents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/apireportingv2incidents-get-openapi.md
- name: Victor Ops
  x-api-slug: victor-ops
  description: VictorOps incident managament software gives DevOps observability,
    collaboration, & real-time alerting, to build, deploy, & operate software. Learn
    more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20023-victorops.jpg
  humanURL: http://victorops.com
  baseURL: https://api.victorops.com//
  tags: VictorOps
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/victorops/master/_listings/victorops/openapi.md
x-common:
- type: x-blog
  url: https://victorops.com/blog/
- type: x-blog-rss
  url: https://victorops.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/victorops
- type: x-email
  url: support@victorops.com
- type: x-email
  url: info@victorops.com
- type: x-email
  url: press@victorops.com
- type: x-email
  url: sales@victorops.com
- type: x-github
  url: https://github.com/victorops
- type: x-pricing
  url: https://victorops.com/pricing/
- type: x-twitter
  url: https://twitter.com/VictorOps
- type: x-website
  url: http://victorops.com
- type: x-website
  url: https://victorops.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---