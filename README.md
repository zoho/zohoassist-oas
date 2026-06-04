# Zoho Assist OpenAPI Specification (OAS)

Welcome to the **Zoho Assist OpenAPI Specification (OAS)** repository. This repository provides the OpenAPI Specification files for Zoho Assist APIs, enabling developers to seamlessly integrate Zoho Assist with their applications using standardized API definitions.

---

## **Overview**

The OpenAPI Specification (OAS) is a standardized format for documenting RESTful APIs. It provides details about API structure, endpoints, request/response formats, and authentication methods in JSON or YAML formats. This repository hosts the OAS files for Zoho Assist APIs to help developers:

- Understand Zoho Assist API endpoints and their usage.
- Generate SDKs in various programming languages.

---

## **Repository Structure**

The repository is organized into the following sections:

- **`ZohoAssist/`**: Contains the OAS files for Zoho Assist APIs.

### Remote Support Sessions

| File | Description |
|------|-------------|
| `createSession.yaml` | Create a new remote support or screen sharing session |
| `scheduleSession.yaml` | Schedule a remote support session |
| `fetchSessionReports.yaml` | Fetch session reports |
| `getSysIdForSessionId.yaml` | Get system ID for a given session ID |

### Session Files & Downloads

| File | Description |
|------|-------------|
| `downloadSessionChats.yaml` | Download chat transcripts from a session |
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

---

## **Getting Started**

### **1. Explore OAS Files**
1. Navigate to the `ZohoAssist/` folder in this repository.
2. Select the OAS file relevant to your use case (e.g., `createSession.yaml` for creating remote support sessions).
3. Use tools like Swagger's API Hub or Postman to import and explore these files.

### **2. Generate SDKs**
Zoho Assist's OAS files can be used to generate SDKs in various programming languages such as Python, Java, and Node.js.

#### Steps:
1. Import the OAS file into Swagger's API Hub:
   - Go to **Swagger API Hub > Design > Import API**.
   - Paste the raw link of the selected OAS file from this repository.
2. Navigate to **Codegen > Client SDK** in Swagger's API Hub.
3. Select your preferred language and download the generated SDK.

---

## **Authentication**

Zoho Assist APIs use OAuth 2.0 for secure authentication via Zoho IAM. All scopes are prefixed by `ZohoAssist.*`.

To authenticate your requests:
1. Obtain your `Client ID`, `Client Secret`, and `Refresh Token` from Zoho's [Developer Console](https://api-console.zoho.com).
2. Configure these credentials in your SDK or application.

---

## **Support**

For any questions or assistance, refer to [Zoho Assist Documentation](https://www.zoho.com/assist/) or contact our support team.

---

Start building powerful integrations with Zoho Assist today!
