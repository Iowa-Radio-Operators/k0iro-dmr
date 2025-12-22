# KO1RO DMR Repeater & Digital Last Heard Dashboard

## Repeater Overview

The KO1RO DMR repeater is now fully online and available for operators throughout the region. This system expands our digital voice capabilities and provides reliable coverage for both analog FM and DMR users.

## Hardware & Configuration

- Repeater: BridgeCom dual-mode (Analog FM + DMR)
- Digital Controller: Repeater Builder STM32-DVM MMDVM Hat
- Time Slots: Dual-slot MMDVM
- Slot Behavior: Time Slot 1 and Time Slot 2 are linked together
- DMR Color Code: 2

## Frequencies

| Mode      | Output       | Input        | Settings              |
|-----------|--------------|--------------|-----------------------|
| Analog FM | 442.4250 MHz | 447.4250 MHz | PL 151.4 Hz (RX & TX) |
| DMR       | 442.4250 MHz | 447.4250 MHz | Color Code 2          |

## DMR IDs

| Description               | ID      |
|---------------------------|---------|
| Repeater ID               | 3215800 |
| Alternate / Group Call ID | 314757  |

## Static Talkgroups (Full-Time)

| Talkgroup ID | Name          | Notes                                   |
|--------------|---------------|------------------------------------------|
| 3119         | Iowa Statewide | Primary statewide calling TG            |
| 31191        | Des Moines     | Central Iowa regional                   |
| 31194        | SW Iowa        | Southwest Iowa / ARES District 4        |
| 31198        | DVN NWS        | Davenport National Weather Service       |
| 31199        | DMX NWS        | Des Moines NWS / SEOC                   |

## Digital Last Heard Dashboard

The Digital Last Heard page provides real-time visibility into repeater activity, including callsigns, talkgroups, signal quality, and system performance.

Access the dashboard here:

https://dmr.k0iro.com/lastheard/

This page automatically refreshes and displays the most recent transmissions received by the repeater.

## Pi-Star API Integration

The Last Heard dashboard retrieves live data from the Pi-Star backend using the following API endpoint:

```text
/pistar/api/last_heard.php