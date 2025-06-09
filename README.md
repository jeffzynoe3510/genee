# Virtual Try-On Application

A Next.js application that provides virtual try-on functionality for clothing items, with size recommendations and shopping features.

## Features

- Virtual mirror with real-time clothing overlay
- Multiple view angles (front, back, left, right)
- AI-powered size recommendations
- Shopping cart and wishlist functionality
- User profile with measurements
- Try-on history

## Prerequisites

- Node.js 18.x or later
- PostgreSQL database
- Google OAuth credentials (for authentication)
- OpenAI API key (for size recommendations)

## Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
DATABASE_URL="postgresql://user:password@localhost:5432/virtual_try_on"
NEXTAUTH_URL="http://localhost:3000"
NEXTAUTH_SECRET="your-secret-key"
GOOGLE_CLIENT_ID="your-google-client-id"
GOOGLE_CLIENT_SECRET="your-google-client-secret"
OPENAI_API_KEY="your-openai-api-key"
```

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Set up the database:
   ```bash
   npx prisma migrate dev
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

- `/src/app` - Next.js app router pages
- `/src/components` - React components
- `/src/lib` - Utility functions and configurations
- `/src/types` - TypeScript type definitions
- `/prisma` - Database schema and migrations

## Technologies Used

- Next.js 13
- React 18
- TypeScript
- Prisma
- NextAuth.js
- Tailwind CSS
- OpenAI API

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.