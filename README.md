# Digital Wedding Invite Portfolio
A responsive, interactive digital wedding invitation web application built with **Next.js, React, TypeScript, and Tailwind CSS**.
The application provides guests with an interactive invitation experience and allows them to submit RSVP responses through a backend workflow using **Google Apps Script and Google Sheets**.

## Live Demo
**[View the Live Wedding Invitation](https://ourweddinginvitation.shwetsh.xyz/)**

---
## About the Project

This project is a personalized digital wedding invitation designed to provide guests with an interactive experience rather than a traditional static invitation.

The application opens with an interactive invitation experience, allowing visitors to interact with the invitation seal and explore wedding and event information.

The project was designed and developed as a real-world application and deployed for public access.

---

## Features

* Interactive wedding invitation opening experience
* Wedding-themed visual design
* Responsive design for mobile, tablet, and desktop
* Personalized wedding content
* Interactive RSVP form
* Guest attendance selection
* Guest information collection
* RSVP submission processing
* RSVP data stored in Google Sheets
* Reusable React components
* Component-based UI architecture
* Public cloud deployment

---

## Application Architecture

```text
                         ┌──────────────────────┐
                         │      Guest/User      │
                         │      Web Browser     │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │        Vercel        │
                         │                      │
                         │       Next.js        │
                         │  React + TypeScript   │
                         │    Tailwind CSS      │
                         └──────────┬───────────┘
                                    │
                              RSVP Submission
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │   Google Apps Script │
                         │       Web App        │
                         │                      │
                         │   RSVP Processing    │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │     Google Sheets    │
                         │                      │
                         │    RSVP Data Store   │
                         └──────────────────────┘
```

### RSVP Data Flow

1. Guest opens the wedding invitation.
2. Guest completes the RSVP form.
3. The React application manages the form state.
4. RSVP data is submitted to the Google Apps Script Web App.
5. Google Apps Script processes the submission.
6. RSVP information is stored in Google Sheets.

---

## Technology Stack

| Layer                | Technology                              |
| -------------------- | --------------------------------------- |
| Framework            | **Next.js**                             |
| UI Library           | **React**                               |
| Language             | **TypeScript**                          |
| Styling              | **Tailwind CSS**                        |
| UI Components        | **shadcn/ui**                           |
| Component Primitives | **Radix UI**                            |
| Icons                | **Lucide React**                        |
| Architecture         | **Next.js App Router**                  |
| Components           | **Reusable React Components**           |
| Forms                | **React State / Controlled Components** |
| RSVP Backend         | **Google Apps Script Web App**          |
| Data Storage         | **Google Sheets**                       |
| Version Control      | **Git + GitHub**                        |
| Deployment           | **Vercel**                              |

---

## Project Structure

```text
Digital-Wedding-Invite-Portfolio/
│
├── app/
│   ├── layout.tsx
│   ├── page.tsx
│   └── ...
│
├── components/
│   ├── RSVPForm.tsx
│   ├── LotusPattern.tsx
│   └── ...
│
├── public/
│   └── ...
│
├── README.md
├── package.json
├── tsconfig.json
└── ...
```

The application uses reusable React components to separate UI responsibilities and keep the codebase maintainable.

---

## RSVP Implementation

The RSVP form allows guests to submit their response through an interactive form.

The form collects:

* Guest name
* Attendance status
* Number of guests
* Personal message

The form is implemented using React state and controlled form inputs.

The submission flow is:

```text
RSVP Form
    │
    ▼
React State
    │
    ▼
Google Apps Script Web App
    │
    ▼
Google Sheets
```

This provides a lightweight backend workflow without requiring a dedicated application server or database infrastructure.

---

## Responsive Design

The application is designed to provide a consistent experience across:

* Mobile devices
* Tablets
* Desktop browsers

The UI uses Tailwind CSS responsive utilities to adapt layouts and components to different screen sizes.

---

## UI Architecture

The application follows a reusable component-based approach.

Common UI responsibilities are separated into React components, allowing individual sections of the invitation to be developed and maintained independently.

The project also uses **shadcn/ui** and **Radix UI** components where appropriate.

---

## Getting Started

### Prerequisites

Make sure you have:

* Node.js installed
* npm installed
* Git installed

### Clone the Repository

```bash
git clone https://github.com/shwetah-git/Digital-Wedding-Invite-Portfolio.git
```

### Navigate to the Project

```bash
cd Digital-Wedding-Invite-Portfolio
```

### Install Dependencies

```bash
npm install
```

### Run the Development Server

```bash
npm run dev
```

The application will be available at:

```text
http://localhost:3000
```

---

## Build for Production

Create a production build:

```bash
npm run build
```

Start the production server:

```bash
npm start
```

---

## Deployment

The application is deployed using **Vercel**.

The production deployment is connected to the GitHub repository, allowing the application to be built and deployed through the Vercel platform.

### Production URL

**https://ourweddinginvitation.shwetsh.xyz/**

---

## Security Considerations

The public repository does not contain private credentials or sensitive configuration.

Any environment-specific configuration should be provided through environment variables rather than committed directly to the repository.

---

## Project Highlights

* Designed and developed the application end-to-end
* Built an interactive invitation experience using React and Next.js
* Implemented responsive UI using Tailwind CSS
* Developed reusable React components
* Implemented RSVP submission workflow
* Integrated Google Apps Script as a lightweight backend
* Used Google Sheets for RSVP data persistence
* Deployed the application to Vercel
* Configured a custom production domain
* Built and deployed a real-world application rather than a static UI mockup

---

## Screenshots
### Invitation landing screen
![Wedding Invitation landing screen](screenshots/Wedding-Invite-Landing-screen.png)

### Cover page bride & groom screen
![Cover page bride & groom screen](screenshots/Cover-page-bride&groom-screen.png)

### Wedding details screen
![Wedding details screen](screenshots/Wedding-details-screen.png)

### Scratch the wedding date screen
![Scratch the wedding date screen](screenshots/Scratch-the-wedding-date-screen.png)

### Reveal the wedding date screen
![Reveal the wedding date screen](screenshots/Reveal-the-wedding-date-screen.png)

### Wedding ceremony details screen
![Wedding ceremony details screen](screenshots/Wedding-ceremony-details-screen.png)

### RSVP form screen
![RSVP form screen](screenshots/RSVP-form-screen.png)
---

## License

This project is intended for personal/event use.

---

### Links

**Live Application:**
https://ourweddinginvitation.shwetsh.xyz/

**GitHub Repository:**
https://github.com/shwetah-git/Digital-Wedding-Invite-Portfolio
