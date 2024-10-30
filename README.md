#	onionPhone
###	A privacy and security oriented Smartphone (& Firmware)

---

##	Core Idea

Similar to how [Tails](https://tails.net) aims to [maximize privacy and security](https://en.wikipedia.org/wiki/Tails_(operating_system)#Features), the need for a *"hardened"* [Android](https://en.wikipedia.org/wiki/Android_(operating_system))™-based [Firmware](https://en.wikipedia.org/wiki/Firmware#Home_and_personal-use_products) is obvious.

- Whilst  [GrapheneOS does make a good job at security](https://en.wikipedia.org/wiki/GrapheneOS#Security_&_Privacy_features), it does not implement a fully transparent torification using [Orbot](https://en.wikipedia.org/wiki/Orbot) from the get-go, and preventing unsafe communication as Tails does.

##	Goal

1. Provide a simple to setup & boot into Android™-based distribution that is as east to get started as Tails.
2. Develop a reference implementation / devkit for support. (aka. design a reference device)

##	Components 

###	[Android](https://source.android.com/)™
As base operating system.
-	Since Android™

###	Preloaded / Replacement Apps:

####    [F-Droid](https://f-droid.org/en/packages/org.fdroid.fdroid/) as preinstalled *"Store"*.
Not only are we not a licensee for [Google Play](https://play.google.com) but also don't want to include it anyway in our ROMs.
- For those that need to download and use Apps from Google Play, (which we disrecommend!) there are options like [Aurora Store](https://f-droid.org/en/packages/com.aurora.store/) that can provide the functionality.
  - We do not guarantee functionality of any App - espechally downloaded through Aurora Store - and won't be able to support any of those. Any issues arising need to be resolved with the Apps' developers' directly.

####    [Orbot](https://orbot.app/en/) for *"torification"* of traffic.

####    [monocles](https://monocles.eu/) [Apps](https://docs.monocles.eu/apps/apps/) which are privacy-focussed.
- [monocles chat](https://f-droid.org/en/packages/de.monocles.chat/) - a XMPP client that supports PGP, OMEMO & OTR encryption.
- [monocles mail](https://f-droid.org/en/packages/de.monocles.mail/) - an eMail client that supports PGP/MIME encryption.

####    VPN Clients
- [WG Tunnel](https://f-droid.org/en/packages/com.zaneschepke.wireguardautotunnel/) for [WireGuard](https://en.wikipedia.org/wiki/WireGuard).
- [OpenVPN for Android](https://f-droid.org/en/packages/de.blinkt.openvpn/) to connect to [OpenVPN](https://en.wikipedia.org/wiki/OpenVPN).

####    Several Utilities to make things easier and/or secure
- [OpenKeychain](https://f-droid.org/en/packages/org.sufficientlysecure.keychain/), a simple App to facilitate OpenPGP encryption, decryption, signing and verifying.
- [Keyoxide](https://f-droid.org/en/packages/org.keyoxide.keyoxide/), a decentralized and privacy-friendly alternative to [keybase](https://keybase.io) in terms of verifying PGP keys.
- [AdAway](https://f-droid.org/en/packages/org.adaway/), a sleek Adblocker.
- [ntfy](https://f-droid.org/en/packages/io.heckel.ntfy/), a client to recieve notifications from [ntfy.sh](https://ntfy.sh) - servers.
- [OnionShare](https://f-droid.org/en/packages/org.onionshare.android.fdroid/), a [suite for collaboration and chat](https://onionshare.org/) via Tor.
- [WebCall](https://f-droid.org/en/packages/timur.webcall.callee/), A WebRTC-based, [End-to-End encrypted (Video-)Calling App](https://timur.mobi/webcall/).
- [Zulip](https://f-droid.org/en/packages/com.zulipmobile/), a self-hosting capable [Group Chat Solution](https://zulip.com/).
- [Ripple](https://f-droid.org/en/packages/info.guardianproject.ripple/), a *"panic button"* to wipe apps and/or devices.
- [baresip+](https://f-droid.org/en/packages/com.tutpro.baresip.plus/), a Open-Source VoIP client.

##	Legal

###	Disclaimers
As per [Google](https://partnermarketinghub.withgoogle.com/brands/android/legal-and-trademarks/legal-requirements/) & [Android](https://developer.android.com/distribute/marketing-tools/brand-guidelines?hl=en) Brand guidelines as well as [Android Developer Terms](https://developer.android.com/legal).
- Android™ is a trademark of Google LLC.

###	Note
onionPhone is *not* officially supported nor endorsed by Google and contains code that does not allow to ship it as Android™, so we only call it Android™-based for that reason as to avoid confusion.
