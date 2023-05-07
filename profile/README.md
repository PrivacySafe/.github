# PrivacySafe

We make an uncompromisingly user-centric digital space, addressing every single major privacy, security and ownership aspect. Our approach is simple: user computation and networking controls are moved onto user-owned devices while servers see no user data and dictate nothing. User installs and runs apps on PrivacySafe client-side platform while utility servers don't know what apps use their utility services.


## 3NWeb protocols

Tech freedom starts with standards. [3NWeb](https://github.com/PrivacySafe/3NWeb-architecture#readme) is a set protocols for client-server communication, formats for data on clients, API's that separate common client side base and custom applications that can run on top of it.

3NWeb client-server protocols are formulated strictly within an Application layer in an OSI networking model, allowing combining with privacy-respecting Transport layer(s) for an absolutely private digital realm. 3NWeb is a "killer app" for onion networks like Tor, and mixnets like Nym. Or more specifically, 3NWeb is a "killer app foundation" that let's user-facing app developers do their amazing work without worring about cryptographic intricacies.


## Federation, the web style

Tech sovereignty and freedom requires federation. There are two architectural ways to deliver federated user experience.

One is a classical federation in which client side delegates to "home server" all of its network activity, namely delivering messages to peer's "home inbox server". Such delegation requires client side to tell the server message destination, it requires to devulge communication metadata to so-called third parties at an Application network layer.

Due to metadata disclosure, classical architecture of federation is viewed as incompatible with privacy. Historically it's been a painful point, cause when one thinks that classical architecture is the only way to deliver federation, then with privacy there is no room for user tech sovereignty. We've seen debate between [Signal](https://signal.org/blog/the-ecosystem-is-moving/) and [Matrix](https://matrix.org/blog/2020/01/02/on-privacy-versus-freedom/) developers. Threema devs don't even consider federated protocols in [their messenger comparison](https://threema.ch/en/messenger-comparison).

Luckily for users there is another architectural way to having federation: the [web-style federation](https://github.com/PrivacySafe/3NWeb-architecture#federated-systems-classical-vs-web-styles). In this architecture client finds and delivers bytes directly into peer's "home inbox server". When such delivery is anonymous, metadata drops to harmless levels at the Application network layer. Direct finding and talking to servers is what web client do, hence this second approach to federation is called web-style. The "Web" part in 3NWeb indicates systematic use of web-style federation.

Web-style federation gives a way to minimize metadata at the Application network layer. This leaves an eavesdropper only with metadata at the Transport network layer, in particular IP addresses. VPNs, onion network and mixnets are transport mechanisms that hide user IP addresses. For an absolute privacy, client side platform should use some of these methods, similarly to how client side Tor and Brave browsers use The Onion Router (Tor) network.


## PrivacySafe implementation

There are three parts:
 - [spec-server](https://github.com/PrivacySafe/spec-server) is a server side implementation of all 3NWeb utility protocols: MailerId, 3NStorage and ASMail. This is a reference implementation with test suites for aforementioned protocols.
 - [PrivacySafe](https://github.com/PrivacySafe/privacysafe-platform-electron) implements a client side platform that is a base for user-facing 3NWeb applications.
 - PrivacySafe 3NWeb applications for system needs like [apps launcher](https://github.com/PrivacySafe/launcher.app.privacysafe.io), [apps installer with updates](https://github.com/PrivacySafe/installer.app.privacysafe.io), and applications for user needs like [contacts](https://github.com/PrivacySafe/contacts.app.privacysafe.io), [inbox](https://github.com/PrivacySafe/inbox.app.privacysafe.io), [files](https://github.com/PrivacySafe/files.app.privacysafe.io).
 
 
 ### Runs on all desktops
 
[v.0.14.74_-_chat_on_mac_and_linux.webm](https://user-images.githubusercontent.com/13634613/236695491-49a386a6-08a8-4d85-b362-f26ce67b5e17.webm)
