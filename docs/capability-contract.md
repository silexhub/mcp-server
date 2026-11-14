# A capability's public contract

[Back to the integration hub](../README.md)

This is the documentation standard for a future SilexHub MCP capability. It is not a list of released tools or an API schema.

| Area | What a user or agent needs to know |
| --- | --- |
| Task | The job, intended result, supported scope, and important limits |
| Input | Required and optional fields, types, units, accepted formats, and bounds |
| Output | Result format, field meanings, and a complete synthetic example |
| Permission | Who may call it, required grants, and how ownership is checked |
| Usage | What is counted, applicable limits, and any published charging rule |
| Failure | Invalid input, denied access, unavailable dependencies, and timeouts |
| Retry | Whether a retry is safe, how duplication is handled, and how to find a result |
| Version | The contract version and changes that affect existing callers |

## Keep outcomes distinguishable

A successful call returns a useful result in the documented format. A rejected or failed call returns a clear failure; a blank artifact must not silently stand in for success. Usage and result retrieval behavior should be explained for both success and failure.

Tools with side effects need an explicit action scope and duplicate-request behavior. Documentation alone does not establish those guarantees; they must be checked against the released service.

## Public examples

Use small synthetic inputs. Show enough of the result for a developer to understand its shape and limitations. Do not include customer records, internal addresses, private configuration, or backend error traces.

A capability is listed as available only after its implementation and connection path pass the [release checks](release-readiness.md).
