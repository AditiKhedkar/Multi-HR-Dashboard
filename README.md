# HR Dashboard
website link 
https://multi-hr-dashboards.netlify.app/dashboard

A comprehensive HR management solution with employee management, leave tracking, and company announcements.

## Features

- **Multi-tenant Architecture**: Company switcher for managing multiple organizations
- **Employee Management**: Complete employee directory with filtering and pagination
- **Leave Management**: Visual tracking of leave balances and usage
- **Announcements**: Company-specific announcements feed
- **Role-based Access Control**: Different permissions for admins and employees

## Tech Stack

- **Frontend**: React, TypeScript, TailwindCSS
- **State Management**: React Context + useReducer for application state
- **Data Visualization**: Recharts for interactive charts
- **API Integration**: Mock API services with simulated network latency
- **Testing**: Jest and React Testing Library
- **CI/CD**: GitHub Actions workflow
- **Containerization**: Docker support

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/hr-dashboard.git
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the development server:
   ```
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`



## Project Structure

```
src/
├── components/       # Reusable UI components
│   ├── announcements/
│   ├── auth/
│   ├── common/
│   ├── employees/
│   ├── layout/
│   └── leaves/
├── context/          # React Context for state management
├── pages/            # Main application pages
├── services/         # Mock API services
└── __tests__/        # Unit and integration tests
```

## Docker

To build and run the application using Docker:

```
# Build the Docker image
docker build -t hr-dashboard .

# Run the container
docker run -p 8080:80 hr-dashboard
```

Then access the application at `http://localhost:8080`

## Testing

Run the test suite:

```
npm test
```

Run tests in watch mode:

```
npm run test:watch
```

## Trade-offs and Future Improvements

### Trade-offs

- Used mock data instead of a real backend to simplify setup
- Limited role-based access to basic admin/employee distinction
- Focused on core HR features rather than comprehensive HR system capabilities

### Future Improvements

- Implement a real backend with database persistence
- Add more granular role-based permissions
- Enhance employee profiles with more details and document management
- Add leave request workflow with approvals
- Implement real-time notifications
- Improve mobile responsiveness for smaller screens
- Add data export capabilities
- Integrate with calendar systems

## License

This project is licensed under the MIT License - see the LICENSE file for details.
