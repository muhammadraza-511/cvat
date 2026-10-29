# Annotation Analytics Assessment Definition of Done

This checklist was created before feature implementation. An item is only complete
when its evidence is recorded beside it.

- [ ] CVAT starts, a superuser exists, and a job displays labelled COCO boxes. Evidence: task ID and image count.
- [ ] The endpoint returns correct database-derived class counts for a known task. Evidence: response and comparison method.
- [ ] An unauthenticated request is rejected. Evidence: status code and reproducible command or test.
- [ ] A user without access to the task is rejected. Evidence: status code and reproducible command or test.
- [ ] The web interface calls the endpoint and renders a matching graph. Evidence: route and manual-test result.
- [ ] A task without relevant annotations has a clear empty state. Evidence: task/route and observed result.
- [ ] A failed request has a clear error state. Evidence: controlled failure method and observed result.
- [ ] The selected additional grouping/filter works and its rationale is documented. Evidence: result and rationale.
- [ ] MO-1 includes five raw runs, median, spread, conditions, and an honest target outcome. Evidence: `docs/objectives.md`.
- [ ] Relevant automated checks pass, or failures and their causes are declared. Evidence: commands and output summary.
- [ ] The Plan decision record states the chosen approach, rejected approach, and cost. Evidence: `docs/plan.md`.
- [ ] All unfinished work is listed below. Evidence: maintained list.
- [ ] A Loom recording under five minutes shows the feature, traces one request, and answers K1-K4 from the submitted code. Evidence: Loom link.

## Unfinished work / known limitations

- Pending implementation.
