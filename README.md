# ContactsHub

ContactsHub is a modern contact management application that allows users to store, organize, and manage their contacts using linked list for data management. Built with Next.js for the frontend and Flask for the backend, it provides a seamless user experience with a robust backend infrastructure.
- Backend: https://github.com/ishola-faazele/dsa-contact-manager-backend
- Frontend: https://github.com/ishola-faazele/contactshub-nextapp
- Linkedlist library: https://github.com/ishola-faazele/knust-coe-dsa-2024-25-group20-linkedlist

## Features
- Add, edit, and delete contacts
- Categorize contacts with labels/tags
- Search and filter contacts
- Secure authentication and authorization
- Responsive and intuitive UI

## Tech Stack
### Frontend:
- **Framework:** Next.js (React)
- **Styling:** TailwindCSS
- **Animations:** Framer Motion
- **Custom Modules:** Custom Linked List Node Module (Published on npm)

### Backend:
- **Language:** Python
- **Framework:** Flask
- **Database:** PostgreSQL
- **Authentication:** JWT, OAuth, etc.
- **Hosting:** Vercel (Frontend), Render (Backend), Docker (Backend Containerization)

## Installation
### Prerequisites
Ensure you have the following installed:
- Node.js & npm
- Python & pip
- PostgreSQL
- Docker

### Setup Backend (Using Docker)
1. Pull the Docker image from the registry:
   ```bash
   docker pull isholafaazele/contactshub-backend:latest
   ```
2. Create an `.env` file with the required environment variables:
   ```env
   DB_HOST=your-db-host
   DB_PORT=5432
   DB_USER=youruser
   DB_PASSWORD=yourpassword
   DB_NAME=contactshub
   SECRET_KEY=your_secret_key
   ```
3. Run the backend container:
   ```bash
   docker run -d --env-file .env -p 5000:5000 your-docker-username/contactshub-backend:latest
   ```
## API Endpoints
| Method | Endpoint       | Description          |
|--------|----------------|------------------------|
| GET    | /api/contacts    | Get all contacts       |
| GET    | /api/contacts:id | Get contact a contact  |
| GET    | /api/user-activities    | Get all user activities       |
| POST   | /api/contacts    | Add a new contact      |
| PUT    | /api/contacts/:id               | Update a contact      |
| PATCH  | /api/contacts/:id/toggle-favorite| adds or remove a contact from favorites|
| PATCH | /api/contacts/:id/set-status | changes status of contact -- active, blocked, bin |
| DELETE | api/contacts/:id | Delete a contact      |

### Setup Frontend
1. Clone the repository:
   ```bash
   git clone https://github.com/ishola-faazele/contactshub-nextapp.git
   ```
3. Navigate to the frontend directory:
   ```bash
   cd contactshub-nextapp
   ```
4. Install dependencies:
   ```bash
   npm install
   ```
5. Install the custom Linked List Node Module:
   ```bash
   npm install knust-compeng-dsa-linkedlist
   ```
6. Run the development server:
   ```bash
   npm run dev
   ```


## Deployment
- **Frontend:** Deployed on Vercel
- **Backend:** Deployed on Render & Docker Hub
- **Database:** Hosted PostgreSQL

## Contributing
1. Fork the repository.
2. Create a new branch (`feature/your-feature`).
3. Commit your changes and push the branch.
4. Open a pull request.

## License
This project is licensed under the MIT License.

## Contact
For any inquiries, reach out at [your-email@example.com](mailto:your-email@example.com).

