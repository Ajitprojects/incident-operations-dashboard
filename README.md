# Incident Operations Dashboard

Explore four fictional incidents in a browser. Change the status filter to see how the incident queue, service counts and response metrics change. Open a row to inspect its timeline.

**Run locally.** Use **Code → Download ZIP**, extract the folder, and open `index.html`. All sample data and calculations are in [one file](index.html).

## Reproduce the numbers

| Status filter | Incidents | Mean time to detection | Mean time to recovery |
| --- | ---: | ---: | ---: |
| All incidents | 4 | 5.8 min | 39.3 min |
| Open | 1 | 4.0 min | — |
| Resolved | 3 | 6.3 min | 39.3 min |

Open **INC-1001**. Its timeline starts at 10:00 UTC, shows detection at 10:03 and recovery at 10:28. That contributes 3 minutes to the detection average and 28 minutes to the recovery average.

The default detection average uses four durations (3, 6, 4 and 10 minutes). The recovery average uses three (28, 50 and 40 minutes). The open incident has no recovery timestamp, so it is excluded from the recovery denominator. An em dash means there are no eligible records.

## Scope

This HTML, CSS and JavaScript demo uses a fixed dataset. Operational experience informed the choice of metrics. AI assisted with implementation and documentation. The example metrics describe the fictional dataset only.
