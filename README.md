# School Management Information System (SMIS)

SMIS is a React and TypeScript school-management interface that runs locally with Vite. The local frontend does not require Firebase, Docker, a database server, or any environment configuration.

## Requirements

- Node.js 22 LTS
- npm

## Run locally

From the project root:

```bash
npm install --prefix frontend
cd frontend
npm run dev
```

Open the local Vite address shown in the terminal.

Use the development account:

- Email: `admin@school.local`
- Password: `admin`

The browser stores only the local session. No schools, users, dashboard records, or audit events are seeded. The interface displays empty states until records have been entered and verified.

## Build

```bash
cd frontend
npm run build
```

## Implementation boundary

The local configuration includes browser-local authentication, role-profile loading, empty dashboard states, and the system navigation. Super Administrators can enroll schools with unique codes, choose an accent colour, select required modules, suspend or activate schools, review audit logs, manage permissions, and change technical settings. These controls persist in browser local storage for local development. No dummy records are included.

Before production use, replace local authentication with a secured production identity service and add appropriate MFA, monitoring, backups, retention policies, migration, and restore tests. Apply the Uganda Data Protection and Privacy Act, 2019 and the requirements for student/minor data.
