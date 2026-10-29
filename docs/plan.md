# Annotation Analytics Assessment Plan

**Starting CVAT SHA:** `5d9c21558fff8d8eb47c6f9577357b0e1ecf97c5`  
**Branch:** `dev-test01`

## Work order and time budget

| Budget | Work | Checkpoint |
| --- | --- | --- |
| 0:00-0:45 | Start CVAT, create a superuser, and import a manageable COCO 2017 validation sample. | A job visibly contains labelled boxes. |
| 0:45-1:30 | Trace CVAT's task, label, and annotation models plus the nearest API and web UI patterns. | Record the chosen model path and endpoint design. |
| 1:30-3:00 | Add Django app `test`; implement a database-aggregated, task-scoped per-class count endpoint and focused tests. | Compare a known task's response with its annotations. |
| 3:00-4:30 | Add a web page/panel that calls the endpoint and renders the counts as a graph. | Labels and graph values match the response. |
| 4:30-5:15 | Implement and verify no-data and failed-request UI states. | Reproducible evidence in the Definition of Done. |
| 5:15-6:00 | Verify existing login and task-access protection; add one useful filter/grouping if cleanly supported. | Rejection-path and grouping evidence. |
| 6:00-6:45 | Measure the endpoint five times, report median and spread, and record raw output. | Measurable objective completed. |
| 6:45-8:00 | Run focused checks, update documentation, complete this decision record, and make a Loom recording under five minutes. | Final evidence and declared limitations. |

## Guardrails

- Use CVAT's existing authentication and task-permission checks; do not bypass or duplicate authorization.
- Aggregate in the database rather than loading annotations into Python.
- Follow the nearest existing CVAT API and web UI conventions.
- Commit each completed slice with a message that states what changed and why.
- Record machine details, sample size, five raw runs, median, and spread for every reported performance number.

## Explicitly deferred

Live WebSocket graph updates and reconnect handling are deferred until requirements
1-4 (endpoint, page, graph, empty state, and error state) are working and evidenced.
If time remains, I will integrate with CVAT's existing update mechanism rather than
introduce a separate socket protocol.

## Decision record (complete before submission)

**Chosen approach:** Pending model/API investigation.  
**Rejected approach:** Pending investigation.  
**Cost of rejecting it:** Pending investigation.

## Plan changes

| When | Change | Reason |
| --- | --- | --- |
| Before implementation | Initial plan committed. | Required before feature code. |
