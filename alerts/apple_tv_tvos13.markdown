---
title: "Apple TV integration incompatible with tvOS 13"
created: 2019-09-07 18:20:03
integrations:
  - apple_tv
github_issue: https://github.com/postlund/pyatv/issues/180
homeassistant: ">0.49"
---

Updating your Apple TV to tvOS 13 will cause the Apple TV media player integration for Home Assistant to no longer work.

The current version of the integration relies on the legacy DAAP-protocol which is being phased out in tvOS 13 in favor of the MediaRemoteTV protocol (MRP) going forward. This is a [known issue](https://github.com/postlund/pyatv/issues/180) which will require an update to the pyatv python library.

If you wish to continue using the Apple TV media player integration in Home Assistant, it's recommended to hold off on installing tvOS 13 at this time. On your Apple TV device, navigate to Settings > System > Software Updates and turn off auto updates.
