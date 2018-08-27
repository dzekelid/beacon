---
name: Google Beacons
x-slug: google-beacons
description: Give your users better location and proximity experiences by providing
  a strong context signal for their devices in the form of Bluetooth low energy (BLE)
  beacons with Eddystone, the open beacon format from Google. The Google beacon platform
  enables you to manage your beacons remotely, integrate with Google services and
  help users devices to discover content and functionality across Android, native
  apps and the web.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
x-kinRank: "9"
x-alexaRank: "0"
tags: Beacon
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/apis.md
specificationVersion: "0.14"
apis:
- name: Google Proximity Beacon - Get Observed Beacon Info
  x-api-slug: v1beta1beaconinfogetforobserved-post
  description: |-
    Given one or more beacon observations, returns any beacon information
    and attachments accessible to your application. Authorize by using the
    [API key](https://developers.google.com/beacons/proximity/how-tos/authorizing#APIKey)
    for the application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beaconinfogetforobserved-post-openapi.md
- name: Google Proximity Beacon - Search Beacons
  x-api-slug: v1beta1beacons-get
  description: |-
    Searches the beacon registry for beacons that match the given search
    criteria. Only those beacons that the client has permission to list
    will be returned.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **viewer**, **Is owner** or **Can edit**
    permissions in the Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beacons-get-openapi.md
- name: Google Proximity Beacon - Register Beacon
  x-api-slug: v1beta1beaconsregister-post
  description: |-
    Registers a previously unregistered beacon given its `advertisedId`.
    These IDs are unique within the system. An ID can be registered only once.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beaconsregister-post-openapi.md
- name: Google Proximity Beacon - Get Beacon Parameters
  x-api-slug: v1beta1eidparams-get
  description: |-
    Gets the Proximity Beacon API's current public key and associated
    parameters used to initiate the Diffie-Hellman key exchange required to
    register a beacon that broadcasts the Eddystone-EID format. This key
    changes periodically; clients may cache it and re-use the same public key
    to provision and register multiple beacons. However, clients should be
    prepared to refresh this key when they encounter an error registering an
    Eddystone-EID beacon.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1eidparams-get-openapi.md
- name: Google Proximity Beacon - Delete Beacon
  x-api-slug: v1beta1beaconname-delete
  description: |-
    Deletes the specified beacon including all diagnostics data for the beacon
    as well as any attachments on the beacon (including those belonging to
    other projects). This operation cannot be undone.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beaconname-delete-openapi.md
- name: Google Proximity Beacon - Get Beacon
  x-api-slug: v1beta1beaconname-get
  description: |-
    Returns detailed information about the specified beacon.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **viewer**, **Is owner** or **Can edit**
    permissions in the Google Developers Console project.

    Requests may supply an Eddystone-EID beacon name in the form:
    `beacons/4!beaconId` where the `beaconId` is the base16 ephemeral ID
    broadcast by the beacon. The returned `Beacon` object will contain the
    beacon's stable Eddystone-UID. Clients not authorized to resolve the
    beacon's ephemeral Eddystone-EID broadcast will receive an error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beaconname-get-openapi.md
- name: Google Proximity Beacon - Update Beacon
  x-api-slug: v1beta1beaconname-put
  description: |-
    Updates the information about the specified beacon. **Any field that you do
    not populate in the submitted beacon will be permanently erased**, so you
    should follow the "read, modify, write" pattern to avoid inadvertently
    destroying data.

    Changes to the beacon status via this method will be  silently ignored.
    To update beacon status, use the separate methods on this API for
    activation, deactivation, and decommissioning.
    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beaconname-put-openapi.md
- name: Google Proximity Beacon - Activate Beacon
  x-api-slug: v1beta1beaconnameactivate-post
  description: |-
    Activates a beacon. A beacon that is active will return information
    and attachment data when queried via `beaconinfo.getforobserved`.
    Calling this method on an already active beacon will do nothing (but
    will return a successful response code).

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beaconnameactivate-post-openapi.md
- name: Google Proximity Beacon - Deactivate Beacon
  x-api-slug: v1beta1beaconnamedeactivate-post
  description: |-
    Deactivates a beacon. Once deactivated, the API will not return
    information nor attachment data for the beacon when queried via
    `beaconinfo.getforobserved`. Calling this method on an already inactive
    beacon will do nothing (but will return a successful response code).

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beaconnamedeactivate-post-openapi.md
- name: Google Proximity Beacon - Decomission Beacon
  x-api-slug: v1beta1beaconnamedecommission-post
  description: |-
    Decommissions the specified beacon in the service. This beacon will no
    longer be returned from `beaconinfo.getforobserved`. This operation is
    permanent -- you will not be able to re-register a beacon with this ID
    again.

    Authenticate using an [OAuth access token](https://developers.google.com/identity/protocols/OAuth2)
    from a signed-in user with **Is owner** or **Can edit** permissions in the
    Google Developers Console project.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-beacons.jpg
  humanURL: https://developers.google.com/beacons/
  baseURL: ://proximitybeacon.googleapis.com//
  tags: Beacons, Sensors, Internet of Things, Google APIs, Stack Network, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/beacon/master/_listings/google-beacons/v1beta1beaconnamedecommission-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.apps.script.execution.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.beacons.stack.network
- type: x-dashboard
  url: https://developers.google.com/beacons/dashboard/
- type: x-website
  url: https://developers.google.com/beacons/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---