# K0IRO DMR Repeater & Digital Last Heard Dashboard

## Repeater Overview

The K0IRO DMR repeater is now fully online and available for operators throughout the region. This system expands our digital voice capabilities and provides reliable coverage for both analog FM and DMR users.

## Digital Last Heard Dashboard

The Digital Last Heard page provides real-time visibility into repeater activity, including callsigns, talkgroups, signal quality, and system performance.

Access the dashboard here:

https://dmr.k0iro.com/lastheard/

This page automatically refreshes and displays the most recent transmissions received by the repeater.

## Pi-Star API Integration

The Last Heard dashboard retrieves live data from the Pi-Star backend using the following API endpoint:

```text
/pistar/api/last_heard.php