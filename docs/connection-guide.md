# Connecting to SilexHub through MCP

[Back to the integration hub](../README.md)

**Status: not released.** This guide explains the intended connection flow. It does not provide an endpoint or a configuration that can be used today.

## Hosted connection: the first planned route

A hosted MCP connection lets a compatible client reach a remotely operated service. When SilexHub releases this route, its documentation will provide:

1. The verified server address and supported transport.
2. Supported clients and the tested configuration for each.
3. The supported authorization flow and how to revoke access.
4. The available capabilities and their input/output contracts.
5. Applicable limits, usage rules, and failure behavior.

Use only the server address and client configuration published with a release. The product website address is not an MCP endpoint.

## Local adapter: a later distribution option

A local adapter is software launched by an MCP client on the user's machine. It may connect onward to a hosted service. We will publish an installation command only after an actual package has been built, tested, and released.

A local adapter is not the SilexHub application, a bundled database, or a self-hostable copy of the hosted backend. Its supported scope will be explicit in its release notes.

## First connection checks

For a released integration, verify that the client can discover the documented capability, complete a small permitted task, and receive the documented output. A refused request must remain refused; reconnecting should not widen access.

Report connection problems with the client and integration versions, a sanitized error, and a synthetic input. Do not post access credentials, session material, or private data in an issue.

## Where to follow availability

Check [SilexHub availability](https://github.com/silexhub/docs/blob/main/reference/availability.md) and the [MCP integration README](../README.md). Configuration will be added to this guide when it is supported.
