# Plan

- CVAT commit cloned: 4a09e27ff869b7aebbfdb07b29c4a34904a0221d
- Machine: GitHub Codespace, 2 vCPU, 7.8 GB RAM, Ubuntu 24.04.5 LTS
- Branch: dev-test01

## Order and time budget (8h)
1. Setup: Docker stack, superuser, COCO subset import (waiting time not counted) - 0h
2. Item 1: GET /api/test/tasks/<id>/annotation-counts, counted in the database - 1.5h
3. Items 2-4: page in cvat-ui, bar chart, empty and error states - 2.5h
4. Item 5: auth, 401 without login, 403 without task access, shown with curl - 0.5h
5. Item 6: speed objective, 5 runs, raw output saved - 1h
6. Item 7: grouping by shape type - 0.5h
7. Items 8-9: WebSocket live update and reconnect - only if time remains
8. Documents, decision record, recording - 1.5h

## Decided to skip up front
- Tracks and tags: only labeled shapes are counted
- Video tasks
- Items 8-9 unless items 1-7 are done and evidenced

## Known constraint
The machine is small (2 vCPU, 2.9 GB free RAM while CVAT runs), so the
imported dataset is a subset of COCO val2017. The exact count is in OBJECTIVES.md.

## Changes to plan
(none yet, each change will be added here with its reason)

## Decision record
(written at the end, only if item 10 is reached)
