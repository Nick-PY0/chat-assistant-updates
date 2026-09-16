# Nexa customer releases

This repository contains customer-only Nexa connector releases and their signed manifests. It does not contain the operator host app, the private provider-key service, or credentials.

## Windows and Android apps

Sign in at https://key-rotation-manager.replit.app/account and use **Customer apps** to download the current Windows EXE or Android APK. Those installers are delivered by the Nexa website; the connector ZIPs below are not substitutes for an installer.

## Signed connector updates

- Stable: customer/stable/releases/
- Preview: customer/preview/releases/

The authorized Nexa service selects the signed update for each installation. Customer connectors validate the manifest signature, target platform, archive size, and SHA-256 before applying it. Published versions are immutable.

Automatic connector updates and their manual controls are separate from replacing an entire Windows or Android application. Android installation may require confirmation.

## Publication boundary

Publish only customer-safe packages here. Operator host releases and their history are maintained privately. Never upload provider keys, GitHub credentials, local databases, owner-runtime packages, or signing private keys.
