# PrivacySafe

We make an uncompromisingly user-centric digital space, addressing every single major privacy, security and ownership aspect. Our approach is simple: user computation is moved onto user-owned devices while servers see no user data and dictate nothing. User installs and runs apps on PrivacySafe client-side platform while utility servers don't know what apps use their utility services.


## 3NWeb protocols

Tech freedom starts with standards. [3NWeb](https://github.com/PrivacySafe/3NWeb-architecture#readme) is a set protocols for client-server communication, formats for data on clients, API's that separate common client side base and custom applications that can run on top of it.

3NWeb client-server protocols are formulated strictly within an Application layer in an OSI networking model, allowing combining with privacy-respecting Transport layer(s) for an absolutely private digital realm. 3NWeb is a "killer app" for onion networks like Tor, and mixnets like Nym. Or more specifically, 3NWeb is a "killer app foundation" that let's user-facing app developers do their amazing work without worring about cryptographic intricacies.


## PrivacySafe implementation

There are three parts:
 - [spec-server](https://github.com/PrivacySafe/spec-server) is a server side implementation of all 3NWeb utility protocols: MailerId, 3NStorage and ASMail. This is a reference implementation with test suites for aforementioned protocols.
 - [PrivacySafe](https://github.com/PrivacySafe/privacysafe-platform-electron) implements a client side platform that is a base for user-facing 3NWeb applications.
 - PrivacySafe 3NWeb applications for system needs like [apps launcher](https://github.com/PrivacySafe/launcher.app.privacysafe.io), [apps installer with updates](https://github.com/PrivacySafe/installer.app.privacysafe.io), and applications for user needs like [contacts](https://github.com/PrivacySafe/contacts.app.privacysafe.io), [inbox](https://github.com/PrivacySafe/inbox.app.privacysafe.io), [files](https://github.com/PrivacySafe/files.app.privacysafe.io).
