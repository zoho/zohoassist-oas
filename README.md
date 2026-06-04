# MCP OAS – Zoho Assist

OpenAPI 3.0 specifications for [Zoho Assist](https://www.zoho.com/assist/) APIs, designed for use with the **Model Context Protocol (MCP)**.

## Overview

This repository contains individual OpenAPI spec files that describe the Zoho Assist REST API endpoints. These specs can be consumed by MCP-compatible tools to enable AI-powered remote support and unattended access workflows.

## API Specifications

### Remote Support Sessions

| File | Description |
|------|-------------|
| `createSession.yaml` | Create a new remote support or screen sharing session |
| `scheduleSession.yaml` | Schedule a remote support session |
| `fetchSessionReports.yaml` | Fetch session reports |
| `getSysIdForSessionId.yaml` | Get system ID for a given session ID |
| `downloadSessionChats.yaml` | Download chat logs from a session |
| `downloadSessionNotes.yaml` | Download notes from a session |
| `downloadSessionRecordings.yaml` | Download session recordings |
| `downloadSessionScreenshots.yaml` | Download session screenshots |

### Unattended Access

| File | Description |
|------|-------------|
| `unattendedSession.yaml` | Create an unattended remote session with a device |
| `unattendedDevicesListFetch.yaml` | List all unattended devices |
| `unattendedDeviceDetailsFetch.yaml` | Fetch details of an unattended device |
| `unattendedDeviceDisplayNameUpdate.yaml` | Update the display name of an unattended device |
| `unattendedGroupsListFetch.yaml` | List all unattended device groups |
| `unattendedGroupsCreate.yaml` | Create a new unattended device group |
| `unattendedGroupsUpdate.yaml` | Update an unattended device group |

### User

| File | Description |
|------|-------------|
| `fetchUserDetails.yaml` | Fetch authenticated user details |

## Usage

Each YAML file is a standalone OpenAPI 3.0 specification. Import them into any OpenAPI-compatible tool or MCP server to interact with the Zoho Assist API.

### Authentication

All endpoints use OAuth 2.0 via Zoho IAM with scopes prefixed by `ZohoAssist.*`.

### Base URL

```
https://assist.zoho.com
```

## License

See [LICENSE](LICENSE) for details.
