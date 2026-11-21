# Engine 4 - Testing & Validation
**Subject:** Software Engineering & SDLC  
**Project:** GoldenHour - Severity Ranking and Hospital Readiness Matching System (Theme: Search and Ranking System)  
**Files in this zip:** 24 (plus this README)  

Folder paths are kept as in the full project, so these files drop straight back into the repo.

## What you must be able to explain

- 67 automated tests: api 30, validation 16, priorityQueue 7, readiness 7, geo 5, client severity 2 (Vitest + Supertest, isolated goldenhour_test database).
- Test table, defect log and root-cause notes are NOT in the code: write them from the test files plus your own run results.
- Version control and final report: README.md, PRESENTATION_SCRIPT.md, .gitignore, package files, .env.example, TypeScript configs.
- realtime-check.cjs is the manual end-to-end check for Socket.IO.
- Note: server/.env (contains secrets) is excluded from every zip; copy .env.example to .env and set JWT_SECRET.

## Files owned by this engine

| File | Lines |
| --- | ---: |
| `.env.example` | 26 |
| `.gitignore` | 11 |
| `PRESENTATION_SCRIPT.md` | 507 |
| `README.md` | 417 |
| `client/package.json` | 35 |
| `client/tests/severity.test.ts` | 19 |
| `client/tsconfig.json` | 21 |
| `client/tsconfig.test.json` | 7 |
| `client/vitest.config.ts` | 8 |
| `package-lock.json` | 6760 |
| `package.json` | 32 |
| `server/package.json` | 56 |
| `server/scripts/realtime-check.cjs` | 210 |
| `server/tests/api.test.ts` | 634 |
| `server/tests/geo.test.ts` | 37 |
| `server/tests/global-setup.ts` | 44 |
| `server/tests/priorityQueue.test.ts` | 88 |
| `server/tests/readiness.test.ts` | 115 |
| `server/tests/setup-env.ts` | 7 |
| `server/tests/test-database.ts` | 11 |
| `server/tests/validation.test.ts` | 177 |
| `server/tsconfig.json` | 22 |
| `server/tsconfig.test.json` | 11 |
| `server/vitest.config.ts` | 14 |

## Files from other engines that these files import

| Needs | Owned by | Used by |
| --- | --- | --- |
| `client/src/lib/severity.ts` | Engine 2 | `severity.test.ts` |
| `server/src/app.ts` | Engine 3 | `api.test.ts` |
| `server/src/services/priorityQueue.ts` | Engine 2 | `priorityQueue.test.ts` |
| `server/src/services/readinessService.ts` | Engine 2 | `readiness.test.ts` |
| `server/src/types.ts` | Engine 2 | `priorityQueue.test.ts` |
| `server/src/utils/geo.ts` | Engine 2 | `geo.test.ts` |
| `server/src/validation/ambulanceSearch.ts` | Engine 3 | `validation.test.ts` |
| `server/src/validation/assignment.ts` | Engine 3 | `validation.test.ts` |
| `server/src/validation/emergency.ts` | Engine 3 | `validation.test.ts` |
| `server/src/validation/hospitalMatch.ts` | Engine 3 | `validation.test.ts` |
| `server/src/validation/hospitalResources.ts` | Engine 3 | `validation.test.ts` |
| `server/src/validation/requestId.ts` | Engine 3 | `validation.test.ts` |
