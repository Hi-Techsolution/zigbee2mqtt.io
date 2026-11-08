---
name: zigbee2mqtt-github-links
description: Catalogue of every GitHub repository referenced in the zigbee2mqtt.io documentation (core Zigbee2MQTT projects, adapter firmware and flashing tools, DIY device firmware, integrations). Use when you need the right upstream repo for a Zigbee2MQTT topic — e.g. "where is the Z-Stack firmware", "which repo holds the device converters", "link to the OTA index", "what flasher tool does the doc use", or when adding/checking GitHub links in the docs.
---

# Zigbee2MQTT GitHub links

The full, categorized list lives in [references/github-links.md](references/github-links.md)
(repository → number of doc files citing it → an example source file). Read it rather than guessing a URL.

## Most important repositories

| Need                                                    | Repository                                            |
| ------------------------------------------------------- | ----------------------------------------------------- |
| Zigbee2MQTT application (issues, releases, source)      | https://github.com/Koenkk/zigbee2mqtt                 |
| This documentation site                                 | https://github.com/Koenkk/zigbee2mqtt.io              |
| Device definitions / converters (adding device support) | https://github.com/Koenkk/zigbee-herdsman-converters  |
| Zigbee stack / adapter drivers                          | https://github.com/Koenkk/zigbee-herdsman             |
| OTA firmware index                                      | https://github.com/Koenkk/zigbee-OTA                  |
| Texas Instruments (Z-Stack) coordinator/router firmware | https://github.com/Koenkk/Z-Stack-firmware            |
| Ember (Silicon Labs) adapter CLI tool                   | https://github.com/Nerivec/ember-zli                  |
| Silicon Labs firmware builds                            | https://github.com/darkxst/silabs-firmware-builder    |
| TI flashing (BSL)                                       | https://github.com/JelmerT/cc2538-bsl                 |
| Home Assistant add-on                                   | https://github.com/zigbee2mqtt/hassio-zigbee2mqtt     |
| New frontend (WindFront)                                | https://github.com/Nerivec/zigbee2mqtt-windfront      |
| External converter dev kit                              | https://github.com/Nerivec/z2m-external-converter-dev |
| User extensions                                         | https://github.com/Koenkk/zigbee2mqtt-user-extensions |

## How to use

1. Look the topic up in `references/github-links.md`; the "Example source" column points to the doc page
   that explains the repo's context — open it if you need details.
2. When editing docs, prefer the canonical casing shown in the catalogue (e.g. `Koenkk/...`, not `koenkk/...`).

## Refreshing the catalogue

After docs change, regenerate it from the repo root:

```bash
python3 -I .claude/skills/zigbee2mqtt-github-links/scripts/extract_links.py .
```
