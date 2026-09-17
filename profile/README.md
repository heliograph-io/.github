## Run it on the machine you cannot reach

Somebody else operates the estate. You know what needs running; they can reach it. Today that work happens as instructions pasted into a chat window and screenshots of output pasted back, and the record of what ran is whatever somebody remembered to paste.

**heliograph** replaces that loop. You publish a step. An operator starts a station on their own machine, with their own flags. The station fetches the step, runs it, and pushes back the whole log, timestamped. No inbound port, no VPN, and no credential of yours on their machine.

The station that runs on their machine is published source, so the thing they are being asked to install is a thing they can read. That is the point rather than a detail: the argument for letting this near your estate is that you can check it.

### The repositories

| | |
|---|---|
| [heliograph](https://github.com/heliograph-io/heliograph) | the CLI, the station, the transports, the MCP server and the agent skill |
| [heliograph-relay](https://github.com/heliograph-io/heliograph-relay) | the relay: stores and forwards sealed messages, and holds no payload private key |
| [heliograph-cloud-docs](https://github.com/heliograph-io/heliograph-cloud-docs) | documentation for the hosted service |

Documentation is at [docs.heliograph.io](https://docs.heliograph.io) and the licensing boundary is at [docs.heliograph.io/licence](https://docs.heliograph.io/licence).

### Three things, and they are not the same thing

**heliograph** is the open project and its tooling. **Heliograph Cloud** is the hosted offering: a proprietary broker, console, archive and alerting. **Heliograph** is the business, a trading name of DBHQ Consulting Ltd.

The relay is one to one, carries every message shape, and is always self-hostable. The broker is many to many, and is never self-hosted. **Payload content is end to end encrypted and passes only through published components.** The proprietary broker handles account, topology and authorisation metadata, and can permit, deny or route a connection attempt. It cannot decrypt or forge a payload, and it takes no part in establishing identity: the fingerprint comparison that pairs two ends happens out of band, between two people.

### Licensing

**heliograph** is Apache 2.0, **heliograph-relay** is FSL-1.1-ALv2 converting to Apache 2.0 two years after each release, and the documentation is CC BY 4.0. Applied on 17 September 2026.

**Every commit published under MIT is still available under MIT, permanently**, and a licence change cannot reach backwards. Fork any of them and MIT is what you have.

Calling the relay open source would be wrong, because fair source is not open source. Calling the broker fair source would be wrong twice over: its source is not published and nothing about it converts on a clock.

The whole statement, including the professional-services grant and why fair source rather than AGPL, is at [docs.heliograph.io/licence](https://docs.heliograph.io/licence).

### Availability

**In development. Coming soon.** Contact us if you are interested: [hello@heliograph.io](mailto:hello@heliograph.io)
