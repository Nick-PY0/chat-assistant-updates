# Nexa customer releases

This repository contains customer-only Nexa connector releases and their signed manifests. It does not contain the operator host app, the private provider-key service, or credentials.

## Windows and Android apps

| App | Version | Download |
| --- | --- | --- |
| Windows x64 | 2.0.2 | [Sign in to Nexa → Customer apps](https://key-rotation-manager.replit.app/account) |
| Android | Existing 2.0.2 (code 12) | [Download APK](https://raw.githubusercontent.com/Nick-PY0/chat-assistant-updates/main/customer/apps/android/2.0.2/Nexa-v2.0.2-release.apk) |

**Windows:** install 2.0.2 once to gain whole-app automatic downloads/staging and manual controls. Automatic installation occurs on a normal restart; an active session is not forcibly restarted. The EXE is currently unsigned with Authenticode. GitHub did not accept the EXE upload through the publishing connection, so the complete verified file is hosted by Nexa, not attached here. The updated website must be published to expose the new controls.

**Android:** the existing APK is mirrored unchanged, not a rebuilt Android release. It still has its existing development Clerk configuration. Automatic APK updates require the external Android source and a new build; Android can require installation confirmation.

Size/hash details are in [Windows installer information](customer/apps/windows/2.0.2/release.json) and [Android installer information](customer/apps/android/2.0.2/release.json). These informational JSON files are not signed connector-update manifests. The connector ZIPs below are not substitutes for native installers.

## Signed connector updates

- Stable: customer/stable/releases/
- Preview: customer/preview/releases/

The authorized Nexa service selects the signed update for each installation. Customer connectors validate the manifest signature, target platform, archive size, and SHA-256 before applying it. Published versions are immutable.

Automatic connector updates and their manual controls are separate from replacing an entire Windows or Android application. Android installation may require confirmation.

## Publication boundary

Publish only customer-safe packages here. Operator host releases and their history are maintained privately. Never upload provider keys, GitHub credentials, local databases, owner-runtime packages, or signing private keys.
