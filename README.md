# TripSquad 🌍
**Development Status:** 🚧 Active Development
> Real-time collaborative trip planning platform where friends can plan vacations together without the chaos of group chats and spreadsheets.

## 📋 Overview

**TripSquad** is a social trip planning application that solves the nightmare of coordinating group travel. Vote on destinations, split expenses, build itineraries, and keep everyone in sync with real-time updates.

## 🚀 Tech Stack

### Frontend
- **Angular 18+** - Standalone components, signals, and modern Angular features
- **NG-ZORRO** - Ant Design component library for Angular
- **RxJS** - Reactive programming for real-time data streams
- **SCSS** - Modular styling with variables and mixins
- **TypeScript** - Type-safe development

### Backend
- **FastAPI** - High-performance Python web framework
- **Supabase** - PostgreSQL database with real-time subscriptions
- **WebSockets** - Real-time chat and live updates
- **Pydantic** - Data validation and serialization

### Additional Tools
- **Google Maps API** - Location services and route planning
- **Currency API** - Real-time exchange rates
- **Weather API** - Forecast integration
- **Jasmine/Karma** - Unit testing
- **Cypress** - E2E testing

## 🏁 Getting Started

### Prerequisites
```bash
# Node.js 18+ and npm
node --version
npm --version

# Angular CLI
npm install -g @angular/cli
```

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/tripsquad.git
cd tripsquad
```

2. Install dependencies
```bash
npm install
```

3. Set up environment variables
```bash
cp src/environments/environment.example.ts src/environments/environment.ts
# Edit environment.ts with your Supabase credentials
```

4. Start development server
```bash
ng serve
```

Navigate to `http://localhost:4200/`

## 🛠️ Development

### Code Scaffolding
```bash
# Generate standalone component
ng generate component features/trip-card --standalone

# Generate service
ng generate service core/services/trip

# Generate pipe
ng generate pipe shared/pipes/currency-converter --standalone

# Generate guard
ng generate guard core/guards/auth
```

### Project Structure
```
src/
├── app/
│   ├── core/           # Services, guards, interceptors
│   ├── features/       # Feature modules (trips, chat, expenses)
│   ├── shared/         # Shared components, pipes, directives
│   └── styles/         # Global SCSS files
├── assets/             # Static assets
└── environments/       # Environment configurations
```

### Key Commands
```bash
# Development server
ng serve

# Build production
ng build --configuration production

# Run tests
ng test

# Run tests with coverage
ng test --code-coverage

# Lint code
ng lint

# Format code
npm run format
```

## 🧪 Testing

### Unit Tests
```bash
# Run tests in watch mode
ng test

# Run tests once (CI)
ng test --watch=false --browsers=ChromeHeadless

# Generate coverage report
ng test --code-coverage
```

### E2E Tests
```bash
# Install Cypress
npm install --save-dev cypress

# Run Cypress
npx cypress open
```

## 📦 Build & Deployment

### Development Build
```bash
ng build
```

### Production Build
```bash
ng build --configuration production
```

Build artifacts will be stored in the `dist/` directory.

## 🔧 Configuration

### NG-ZORRO Theme
Customize Ant Design theme in `src/styles.scss`:
```scss
$primary-color: #2c3e50;
$success-color: #27ae60;
```

### Environment Variables
Configure in `src/environments/environment.ts`:
- Supabase URL and anon key
- API endpoints
- Google Maps API key
- Feature flags

## 📚 Key Features

- **Real-time Chat** - WebSocket-powered group messaging
- **Expense Splitting** - Track and split costs automatically
- **Destination Voting** - Democratic trip planning
- **Collaborative Itinerary** - Drag-and-drop schedule builder
- **Live Presence** - See who's online and planning
- **Smart Notifications** - Stay updated on important changes

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Angular CLI](https://github.com/angular/angular-cli) version 20.3.3
- UI components from [NG-ZORRO](https://ng.ant.design)
- Real-time powered by [Supabase](https://supabase.com)

## 📞 Support

For issues and questions:
- Open an issue on GitHub
- Check the [documentation](./docs)
- Review [Angular CLI docs](https://angular.dev/tools/cli)

---