---
layout: bidder
title: Nexverse
description: Prebid Nexverse Bidder Adapter
biddercode: nexverse
tcfeu_supported: false
dsa_supported: true
gvl_id: none
usp_supported: true
coppa_supported: true
schain_supported: true
dchain_supported: false
userId: all
media_types: banner, video, native
safeframes_ok: true
deals_supported: true
floors_supported: true
fpd_supported: true
pbjs: true
pbs: false
prebid_member: false
multiformat_supported: will-bid-on-one
ortb_blocking_supported: false
privacy_sandbox: no
sidebarType: 1
---


### Nexverse Adapter

The Nexverse adapter requires some initial setup. For assistance or setup instructions, please contact us at [support@nexverse.ai](mailto:support@nexverse.ai).

### Supported Media Types

The Nexverse adapter supports the following media types:

- Banner
- Video
- Native

### Configuration

To configure the Nexverse adapter, you will need the following parameters:

| Name   | Scope    | Description              | Example    | Type   |
|--------|----------|--------------------------|------------|--------|
| uid    | required | Publisher's unique ID     | "12345"    | string |
| pubId | required | Publisher ID              | "54321"    | string |
| pubEpid   | optional | Publisher's unique EPID   | "epid123"  | string |
| adPlacementId   | optional | The unique placement ID for the publisher   | "12345"  | string |
| adPlacementName   | optional | The unique placment Name for the publisher   | "IN_abc.com_mid_300x250"  | string |
| siteName   | optional | The Site Name of the publisher   | "nexverse.ai"  | string |
| siteId   | optional | The Site ID for the publisher   | "12"  | string |
| date   | optional | The Placement Creation Date(YYYY-MM-DD)   | "2024-01-01"  | string |


### Test Parameters

You can test the Nexverse adapter with the following test parameters:

```javascript
var adUnits = [
  {
    code: 'div-ad-1',
    mediaTypes: {
      banner: {
        sizes: [[300, 250], [320, 50]],
      },
    },
    bids: [
      {
        bidder: 'nexverse',
        params: {
          uid: '12345',
          pubId: '54321',
          pubEpid: 'epid123',
          adPlacementId: '12345',
          adPlacementName: 'IN_abc.com_mid_300x250',
          siteName: 'nexverse.ai',
          siteId: '12',
          date: '2024-01-01'
        },
      },
    ],
  },
];
```

### GDPR, CCPA, COPPA Support

Nexverse complies with GDPR, CCPA, and COPPA regulations. If you have further questions regarding compliance, feel free to reach out to us.
