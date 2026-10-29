# S01E03 · what it shows

Public deliverable for MEGA.dev challenge [what it shows](https://hq.mega.dev/challenges/what-it-shows).

## Findings in #4471

The desk merged 412 unique date reports into one known ticket. The kb cause logic splits them into two problems:

| cause | reports | meaning |
| --- | ---: | --- |
| `parser` | 379 | Shared parser reads month-first; day-first tenants get flipped dates |
| `hint` | 33 | booking-v3 shows `MM/DD/YYYY` while the form still reads day-first |

GitHub issues in this repo are the tickets for those problems.

## Deliverables

- Issues: one per problem, with report counts
- Page (source): `support-kb/src/routes/kb/incidents/4471-problems/+page.svx`
- Page (as the desk sees it): `rendered/kb/incidents/4471-problems/index.html`

The `support-kb/` tree is the course’s kb export, plus the signed page above.
