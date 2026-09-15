# Nexa — current downloads

Nexa has one login. Customers use their own approved dashboard; the owner
controls admission and permissions for the private ET group.

## Which download do I need?

| Download | Who it is for |
| --- | --- |
| Nexa customer desktop 2.0.1 — Windows x64 EXE **(upload pending)** | The application is built, but its installer is not yet downloadable from this repository. It includes its own login/dashboard window and local runtime. |
| [Owner desktop update 1.10.9](releases/chat-1.10.9.zip) | The existing owner desktop. Prefer its built-in update screen, which verifies the signed update manifest. |

The customer EXE includes the customer connector. It does **not** contain the
owner dashboard, the owner's password, or the publisher's credentials.

### Customer access

1. Run the Windows application and log in or create an account inside its window.
2. Request access, or accept the owner's invitation.
3. Wait for the owner to approve access and assign permissions.
4. Use the allowed dashboard sections. Connect this computer only when device
   access has been enabled for the account.

Downloading the application does not bypass approval. Customer conversations,
devices, credentials, and installations are not shared with other customers
simply because they belong to ET.

Login, approval, synchronization, and hosted AI require an internet connection.
The local runtime is included; hosted services are not offline services.

### Owner access

Complete the protected, one-time owner account link, then manage invitations,
requests, members, and permissions from **Manage access** in your dashboard.
Ownership is never given automatically to the first public signup.

For a verified owner-account sign-in, the owner desktop update removes the
independent 15-minute admin timer. Administration follows that sign-in, while
explicit Lock, sign-out, password changes, and session expiration continue to
revoke access. The matching cloud release and protected owner setup are required
for this account bridge; existing desktop password access remains available.

### Windows publisher notice

The pending customer executable is not Authenticode-signed. It was built and
inspected on Linux, not execution-tested on Windows. Windows may show an
unrecognized-publisher or SmartScreen warning. An update-manifest signature is
not a Windows publisher signature. When the download is published, use only its
official download and compare its SHA-256:

`72b2b8dcb30cb4d6604bbdfc01a1d6b039d8b14b1430460c1e0e6a09e64bbfe3`

No customer Windows EXE is currently published here; the source-code update is
not a substitute for the executable download.

## Other maintained downloads

- [Customer connector 2.0.0 — stable ZIP](customer/stable/releases/nexa-customer-2.0.0.zip)
- [Customer connector 2.0.0 — preview ZIP](customer/preview/releases/nexa-customer-2.0.0.zip)
- [Signed owner update manifest](latest.json)
- [Source code and setup documentation](https://github.com/Nick-PY0/chat-assistant-codex)

These connector ZIPs are for manual/advanced setups; the customer Windows EXE
is the normal desktop download. The connector and desktop application have
separate version numbers.

Older files, release tags, and history are retained for existing installations.
They are intentionally not featured as current downloads. The separately
maintained Android APK is unchanged.

Publishing source or packages to GitHub does not publish the cloud website or
install an update on an existing computer. The matching cloud release and the
protected owner-linking step must be completed before onboarding customers.