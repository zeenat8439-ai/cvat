# Objectives

Machine: GitHub Codespace, 2 vCPU, 7.8 GB RAM, Ubuntu 24.04.5 LTS
CVAT SHA: 4a09e27ff869b7aebbfdb07b29c4a34904a0221d
Images imported: (fill in after import)

| ID | Field | Entry |
|---|---|---|
| MO-1 | What is measured | Server response time of GET /api/test/tasks/<id>/annotation-counts |
| | How | curl -w "%{time_total}" run 5 times, raw output saved in docs/raw/mo1.txt |
| | Target | Median of 5 runs at or below 300 ms (to be justified after a first look at the numbers) |
| | Conditions | Codespace stack, sample data subset, authenticated request, nothing else running, warm cache |
| | Not included | First request after a cold start, video tasks |

## Results
(raw output, median and spread go here after measuring)
