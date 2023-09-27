# AppleTV tvOS VPN and Secure DNS Profiles

AppleTV tvOS 17+ VPN Profiles (mobileconfig) with support of IKEv2 IPSec PPP L2TP PPTP and Secure DNS-over-TLS/QUIC and DNS-over-HTTPS

## Releases

⚡️ Coming Soon ⚡️

## Goals

- VPN Profiles for protocols: [com.apple.vpn.managed](https://github.com/apple/device-management/blob/72c2a0a69f7dfad97f1a7d5733154e81de4e7448/mdm/profiles/com.apple.vpn.managed.yaml)
  - IKEv2 ✅ (tested, works)
  - IPSec
  - PPP
  - L2TP
  - PPTP
  - WireGuard
- Secure DNS Settings [com.apple.dnsSettings.managed.yaml](https://github.com/apple/device-management/blob/72c2a0a69f7dfad97f1a7d5733154e81de4e7448/mdm/profiles/com.apple.dnsSettings.managed.yaml)
  - DNS-over-TLS/QUIC 
  - DNS-over-HTTPS ✅ (tested, works)
- Secure DNS over VPN ❌ (tested, doesn't work, not supported?)
  > Apple's documentation says it is supported on tvOS 17+ but it doesn't install and in the [mdm profile yaml tvOS doesn't seem to be listed (only iOS and macOS)](https://github.com/apple/device-management/blob/72c2a0a69f7dfad97f1a7d5733154e81de4e7448/mdm/profiles/com.apple.vpn.managed.yaml#L1178-L1194) which [contradicts their docs](https://developer.apple.com/documentation/devicemanagement/vpn/dns)

## Documentation

### Apple Official Device Management spec

- https://github.com/apple/device-management/blob/release/mdm/profiles/com.apple.vpn.managed.yaml

### Apple Official VPN tvOS 17+ Documentation

- ✅ https://developer.apple.com/documentation/devicemanagement/vpn
- ✅ https://developer.apple.com/documentation/devicemanagement/vpn/ikev2
- ❌ https://developer.apple.com/documentation/devicemanagement/vpn/dns
  - *Do VPN DNS settings work in tvOS 17+? Couldn't make work, profile doesn't install if set*

### Other Official Reference 

- https://support.apple.com/guide/deployment/ikev2-settings-dep4ce9487d/web

### Profile Generation Tooling

- Apple Configurator 2
- [iMazing Profile Editor](https://imazing.com/profile-editor)
- ~https://github.com/timsutton/make-profile-pkg~

### Guides
- TODO: Add OS Repo tool 
- https://imazing.com/guides/how-to-create-or-edit-apple-configuration-profiles
- https://imazing.com/guides/apple-device-management-glossary#mdm


### Licensing

MIT 2023 Gaston Morixe
