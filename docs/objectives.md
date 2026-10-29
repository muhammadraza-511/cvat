# Annotation Analytics Assessment Objectives

## Environment record

| Field | Value |
| --- | --- |
| CVAT starting commit SHA | `5d9c21558fff8d8eb47c6f9577357b0e1ecf97c5` |
| Operating system | Pending setup |
| CPU | Pending setup |
| RAM | Pending setup |
| Sample data | COCO 2017 validation; image count pending import |

## MO-1: endpoint response time

| Field | Entry |
| --- | --- |
| What is measured | Server response time of the authenticated per-class annotation-count endpoint for one populated task. |
| How | After one warm-up request, send five authenticated requests from the same local machine and record elapsed time in milliseconds. |
| Target | Median at or below 250 ms. |
| Conditions | Local Docker CVAT stack, warm application and database, documented COCO sample size, authenticated user with task access, and no intentional CPU-heavy workload. |
| Not included | Docker cold start, browser rendering, annotation import, and WebSocket updates. |
| Justification | A task-scoped database aggregate and small response should be consistently fast on a local development stack; the target still permits normal machine variance. |

## Raw measurements

| Run | Elapsed ms | Notes |
| --- | ---: | --- |
| 1 | Pending | |
| 2 | Pending | |
| 3 | Pending | |
| 4 | Pending | |
| 5 | Pending | |

**Median:** Pending  
**Spread (min-max):** Pending  
**Target outcome:** Pending
