# External PSK Issues

# Implementation difficulties 

TODO: implementation difficulties, differentiating between stack and application developers. (Maybe summarize existing stack behavior?)

# PSK Provisioning Mechanisms

TODO: what's done in practice?

# External PSK Privacy Properties

Against a passive attacker AdvP or active attacker AdvA, desired privacy properties might include:

- Confidentiality: AdvP should learn no information about the external PSK or its identifier. Similarly, AdvA should be unable to replay ClientHello messages and learn information about the PSK.
- Unlinkability: AdvP should be unable to link two or more connections together that use the same external PSK. 
- XXX

Unlinkability for the PSK receiver, i.e., ensuring that the recipient of a ClientHello with a given PSK cannot link the PSK to another prior session, is out of scope. PSKs are explicitly designed to support mutual authentication.
