# Awesome-Video-Calling-Voip

# Top Video Calling & VoIP Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Real-Time Communication, WebRTC Infrastructure & Self-Hosted Telephony*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Video Calling & VoIP**. These tools enable real-time audio and video communication — from browser-based conferencing to SIP telephony and peer-to-peer mesh networks.

**Examples** include Skype, Zoom, Google Meet, Microsoft Teams, FaceTime, WhatsApp, Viber, Telegram, Discord, and Signal (the category leaders).

**Open-source emphasis**: Real-time communication is one of the strongest open-source domains. **Jitsi Meet**, **BigBlueButton**, **Jami**, **Linphone**, and **La Suite Meet** provide production-grade alternatives to commercial platforms, with **Jitsi** leading for general-purpose rooms and **BigBlueButton** dominating education . This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Zoom](https://zoom.us/)**  
  The dominant video conferencing platform with robust features, AI Companion, and enterprise integrations. Free tier limits group meetings to 40 minutes. Paid plans from $14.99/month .

- **[Microsoft Teams](https://www.microsoft.com/microsoft-teams/)**  
  Enterprise collaboration hub integrating chat, meetings, calling, and Office 365. Bundled with Microsoft 365 subscriptions.

- **[Google Meet](https://meet.google.com/)**  
  Browser-based video conferencing integrated with Google Workspace. Free tier limits group calls to 60 minutes .

- **[Skype](https://www.skype.com/)**  
  Veteran VoIP and video calling service (now Microsoft). Free calling between Skype users; paid options for calling phones.

- **[FaceTime](https://support.apple.com/facetime)**  
  Apple's native video calling with end-to-end encryption. Exclusive to Apple devices; supports group calls up to 32 people.

- **[WhatsApp](https://www.whatsapp.com/)**  
  Messaging app with voice and video calling. End-to-end encrypted by default. Owned by Meta.

- **[Telegram](https://telegram.org/)**  
  Cloud-based messaging with voice/video calls, group calls, and screen sharing. Free with premium tier for advanced features.

- **[Discord](https://discord.com/)**  
  Voice, video, and text communication platform popular with gaming and communities. Free with Nitro subscription for enhanced features.

- **[Signal](https://signal.org/)**  
  Privacy-focused messaging and calling with end-to-end encryption. Non-profit, no ads, no tracking. Free.

## Open-Source GitHub Projects

- **[Jitsi Meet](https://github.com/jitsi/jitsi-meet)**  
  **The leading open-source video conferencing platform**, Apache-2.0 licensed . WebRTC-based with Jitsi Videobridge SFU for scalable multi-user conferences. **No account required** — start a meeting instantly by visiting meet.jit.si and typing a room name . Features screen sharing, recording, virtual backgrounds, chat, hand raising, and Etherpad integration . **Self-hostable with Docker** or Debian packages . No time limits, no participant caps (limited by server capacity) . **The de facto open-source Zoom alternative** for general-purpose meetings .

- **[BigBlueButton](https://github.com/bigbluebutton/bigbluebutton)**  
  **The leading open-source platform for online teaching and training**, LGPL-3.0 licensed . Built for education with whiteboard, breakout rooms, polling, emoji reactions, and **LTI integration with Moodle and other LMS platforms** . Uses mediasoup SFU with FreeSWITCH for audio . **The gold standard for virtual classrooms** — designed for teaching interaction, not just meetings . Requires dedicated server resources and more complex deployment than Jitsi .

- **[Jami](https://git.jami.net/savoirfairelinux/jami-project)**  
  **The only genuine peer-to-peer open-source video calling solution**, GPL licensed . **No server required** — accounts are cryptographic identities stored on device, peers find each other over a distributed hash table, and media flows directly between participants . Supports audio/video calls, messaging, screen sharing, and file transfer . Available on Linux, Windows, macOS, Android, and iOS . **The best choice for small groups where maximum privacy and the absence of any server is the actual requirement** — but group video is limited by upload speeds and NAT traversal success .

- **[Linphone](https://github.com/BelledonneCommunications/linphone-desktop)**  
  **The leading open-source VoIP softphone and SIP client**, GPL licensed . Developed by Belledonne Communications (France) since 2010. Features HD audio/video calls, instant messaging, file sharing, group calls, and video conferencing . **Enterprise-ready** with SSO authentication, LDAP/CardDAV directory integration, and compatibility with existing IPBX systems (Alcatel-Lucent Enterprise, Mitel) . Available on Linux, macOS, Windows, iOS, and Android . **The best choice for organizations wanting open-source SIP telephony** to replace proprietary VoIP systems.

- **[La Suite Meet](https://github.com/suitenumerique/meet)**  
  **Modern open-source video conferencing app powered by LiveKit**, MIT licensed with 2,392+ GitHub stars . Built with Django and React by the French government's digital suite (La Suite Numérique) . Features HD video calls, screen sharing, and chat . **Positioned as a sovereign European alternative** for public sector and organizations wanting modern UX with LiveKit's distributed architecture . Actively developed with strong government backing.

- **[eduMEET](https://github.com/edumeet/edumeet)**  
  **Open-source video conferencing built by and for the research and education community**, now self-sustaining under the Commons Conservancy . Browser-based with no client installation required. **Supports federated architecture** — NRENs can share distributed resources for larger meetings and resilience . Deployed across European research networks including GARR (Italy), PCSS (Poland), and Helmholtz Cloud (Germany) . **The best choice for R&E institutions** wanting sovereign, community-governed infrastructure.

- **[Nextcloud Talk](https://github.com/nextcloud/spreed)**  
  **Video conferencing integrated with Nextcloud**, AGPL licensed . Built on Janus SFU via the High Performance Backend (HPB) for scale . **Best for teams already using Nextcloud** — chat, video calls, and screen sharing within the same platform . Small groups work without HPB; dozens with it .

- **[Galene](https://github.com/jech/galene)**  
  **Lightweight, easy-to-deploy video conferencing server** requiring moderate server resources . Go-based. **The simplest self-hosted option** for small teams wanting minimal operational overhead.

- **[MiroTalk P2P](https://github.com/mirotalk/mirotalk)**  
  **Simple, secure, fast real-time video conferences** up to 4K/60fps, AGPL-3.0 licensed . Compatible with all browsers and platforms. **Peer-to-peer architecture** — no SFU required for small calls. Also available as **MiroTalk SFU** for scalable conferences and **MiroTalk C2C** for embeddable cam-to-cam calls .

- **[plugNmeet](https://github.com/mynaparrot/plugNmeet-server)**  
  **Scalable and high-performance web conferencing system**, Docker/Go-based . Built on LiveKit with a focus on embedding and API-driven integration. **Best for developers building custom conferencing into applications**.

### The Building Blocks: WebRTC Media Servers

For developers building their own conferencing platforms, these are the media layers:

- **[mediasoup](https://github.com/versatica/mediasoup)**  
  **High-performance Node.js SFU library** powering BigBlueButton . C++ core with Node.js signaling. **The best choice for building custom WebRTC applications** with maximum performance . 8-core server can handle 4000+ audio or 800+ video streams .

- **[Janus](https://github.com/meetecho/janus-gateway)**  
  **General-purpose, plugin-based WebRTC server**, GPL-3.0 licensed . Supports VideoRoom, VideoCall, SIP gateway, and streaming plugins . **Best for flexible, multi-purpose deployments** requiring SIP integration or streaming . Powers Nextcloud Talk's HPB .

- **[LiveKit](https://github.com/livekit/livekit)**  
  **Cloud-native WebRTC platform** with distributed architecture and horizontal scaling . Go-based with ETCD control plane. **Powers La Suite Meet** and supports 100K+ concurrent users across 100-node clusters . **Best for large-scale, cloud-native deployments** .

- **[Jitsi Videobridge](https://github.com/jitsi/jitsi-videobridge)**  
  **The SFU powering Jitsi Meet**, Apache-2.0 licensed . Can be used standalone with custom signaling .

**Frameworks for building custom video calling solutions**: Choose based on use case and scale. **Jitsi Meet** for general-purpose meetings with the fastest deployment path . **BigBlueButton** for education and training with LMS integration . **Jami** for maximum privacy with no server infrastructure . **Linphone** for SIP telephony and enterprise VoIP . **La Suite Meet** for modern UX with LiveKit's distributed architecture . For building custom platforms: **mediasoup** for high-performance SFU , **Janus** for plugin flexibility , **LiveKit** for cloud-native scale . Note that **TURN servers (Coturn)** are essential for NAT traversal — without them, calls fail for users behind symmetric NAT or corporate firewalls .

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Video calling tools handle sensitive communications. Self-hosted solutions require proper security hardening, TURN server configuration for NAT traversal, and understanding of WebRTC port requirements .
- **Bandwidth costs scale quadratically** with SFU deployments — 10 participants with cameras means 10 streams in and 90 streams out .
- **Jami's peer-to-peer model** means no server infrastructure, but group video is limited by upload speeds and NAT traversal success .
- The open-source ecosystem provides strong conferencing, telephony, and media server foundations, but **enterprise support, global infrastructure, and AI features** remain primarily commercial offerings.

---

**Made for remote teams, educators, privacy advocates, and developers building real-time communication.**  
Let's make video calling more open, transparent, and privacy-respecting.
