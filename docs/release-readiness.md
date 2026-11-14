# When an MCP integration is ready

[Back to the integration hub](../README.md)

The MCP repository can exist before the service is released. A service is marked usable only when the following have been verified for a real capability.

- A concrete task has an implemented input/output contract and a useful result.
- A real MCP client can discover and call it through the documented connection path.
- Valid input succeeds; invalid input produces the documented error.
- Unauthorized and cross-account requests cannot retrieve another user's result or execute an action.
- Any applicable usage accounting, duplicate requests, retries, and failure outcomes match the published rules.
- A tested quick start identifies the actual endpoint or package version and supported client.
- Public examples use synthetic data; the release contains only reviewed public files.

Record what was checked, which version was tested, and any remaining limitations. A repository, screenshot, or mock response alone does not establish production availability.

## Publication sequence

Validate the smallest real workflow first. Then publish its connection guide and capability contract, update the [availability page](https://github.com/silexhub/docs/blob/main/reference/availability.md), and link the release from the [developer hub](https://github.com/silexhub/silexhub).

Additional SDKs, standalone examples, or client-specific repositories follow demonstrated distribution needs. They are not prerequisites for the first hosted integration.
