# Reflect - A Modern Journaling Application

## Overview
Reflect is a feature-rich journaling application that helps users document their thoughts, track their moods, and organize their entries in collections. Built with modern web technologies, it provides a secure and intuitive platform for personal reflection and emotional tracking.

## Features
- 📝 **Rich Text Editor**: Express yourself with a powerful editor supporting markdown, formatting, and more
- ✨ **Daily Inspiration**: Get inspired with daily prompts and mood-based imagery
- 🔒 **Secure & Private**: Enterprise-grade security with Clerk authentication
- 📊 **Mood Analytics**: Track and visualize your emotional journey
- 📁 **Collections**: Organize your journal entries into custom collections
- 🎨 **Modern UI**: Beautiful and responsive design using Tailwind CSS and Shadcn UI
- 📱 **Mobile Friendly**: Fully responsive design for all devices

## Tech Stack
- **Framework**: Next.js 14 with App Router
- **Frontend**: React, Tailwind CSS, Shadcn UI
- **Backend**: Next.js API Routes
- **Database**: PostgreSQL with Prisma ORM
- **Authentication**: Clerk
- **Security**: ArcJet
- **Hosting**: Neon Database (PostgreSQL)
- **UI Components**: 
  - React Hook Form for form handling
  - React Quill for rich text editing
  - Lucide Icons
  - Sonner for toast notifications

## Getting Started

### Prerequisites
- Node.js 18+ 
- npm/yarn
- PostgreSQL database

### Installation

1. Clone the repository
```bash
git clone https://github.com/ashk6645/Reflect.git
cd Reflect
```

2. Install dependencies
```bash
npm install
# or
yarn install
```

3. Set up environment variables
Create a `.env` file in the root directory and add the following variables:
```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard
DATABASE_URL=your_postgresql_database_url
PIXABAY_API_KEY=your_pixabay_api_key
ARCJET_KEY=your_arcjet_key
```

4. Initialize the database
```bash
npx prisma generate
npx prisma db push
```

5. Run the development server
```bash
npm run dev
# or
yarn dev
```

The application will be available at `http://localhost:3000`

## Project Structure
```
journal-app/
├── actions/         # Server actions for data operations
├── app/            # Next.js app router pages and layouts
├── components/     # Reusable React components
├── hooks/         # Custom React hooks
├── lib/           # Utility functions and configurations
├── prisma/        # Database schema and migrations
└── public/        # Static assets
```

## Features in Detail

### Authentication
- Secure user authentication powered by Clerk
- Protected routes and API endpoints
- User profile management

### Journal Entries
- Rich text editor for writing entries
- Mood selection for each entry
- Auto-save draft functionality
- Collection organization

### Analytics
- Mood tracking visualization
- Entry statistics
- Collection insights

### Collections
- Create and manage collections
- Organize entries into collections
- Collection-specific views

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- [Next.js](https://nextjs.org/)
- [Clerk](https://clerk.dev/)
- [Shadcn UI](https://ui.shadcn.com/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Prisma](https://www.prisma.io/)
- [Neon Database](https://neon.tech/)