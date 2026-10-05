# Problem 1

## User Story Statement

- **As an** API consumer / data analyst
- **I want to** consume God APIs (Greek, Roman & Nordic), filter gods whose names start with a requested letter, convert each filtered god name into a decimal representation, and return the sum of those values
- **So that** I can perform cross-pantheon analysis and aggregate mythology data for research, reporting, or educational applications.

**Notes:**

- Decimal conversion: For each god name, each character is converted to its Unicode integer value and those integers are concatenated as strings (for example, `Zeus` -> `90101117115`). The final result is the numeric sum of all per-name string representations.
- Case sensitivity: The `filter` parameter accepts exactly one Unicode code point and matching is case-sensitive. The documented source data returns god names with uppercase initial letters, such as `Nike`, `Nemesis`, `Neptun`, and `Njord`, so `filter=N` is the meaningful value for the documented aggregate examples. A lowercase `filter=n` is valid but returns no matches for the current documented data.
- HTTP timeouts: Outbound source calls use bounded connect and read timeouts with one attempt per source and no automatic retries; aggregation continues with the sources that return in time. When every selected source times out or fails, the response is HTTP 200 with `sum` `"0"`.
- Acceptance criteria (happy path): Given the God Analysis API is available at `/api/v1` and outbound source calls use bounded connect and read timeouts, a `GET /api/v1/gods/stats/sum?filter=N&sources=greek,roman,nordic` request returns HTTP 200 with a JSON object whose `sum` field is `"78179288397447443426"`.
- Data sources:
  - Greek API: https://my-json-server.typicode.com/jabrena/latency-problems/greek
  - Roman API: https://my-json-server.typicode.com/jabrena/latency-problems/roman
  - Nordic API: https://my-json-server.typicode.com/jabrena/latency-problems/nordic
