# Get in Touch - Contact Form Application

A modern, responsive contact form application built with React, Tailwind CSS, and MongoDB. Features a beautiful UI with animations, form validation, and secure data storage.

## Features

- 🎨 Modern UI with gradient backgrounds and animations
- 📱 Fully responsive design
- ✨ Lucide React icons
- 🔄 Real-time form validation
- 🗄️ MongoDB data storage
- 🚀 Loading states and success/error feedback
- 🔒 Secure API endpoints
- ☁️ Vercel deployment ready

## Tech Stack

- **Frontend**: React 19, Vite, Tailwind CSS v3.4
- **Backend**: Express.js, Node.js
- **Database**: MongoDB
- **Icons**: Lucide React
- **Deployment**: Vercel

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/bezabihz/getintouch.git
cd getintouch
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Environment Variables

Create a `.env` file in the root directory:

```bash
cp .env.example .env
```

Update the `.env` file with your MongoDB connection string:

```env
MONGODB_URI=mongodb+srv://your-username:your-password@your-cluster.mongodb.net/getintouch?retryWrites=true&w=majority
PORT=3001
```

### 4. MongoDB Setup

1. Create a free MongoDB Atlas account at [mongodb.com](https://mongodb.com)
2. Create a new cluster
3. Create a database user
4. Get your connection string
5. Replace the placeholder in `.env` with your actual connection string

### 5. Development

Run the development server:

```bash
# Terminal 1: Start the API server
npm run server

# Terminal 2: Start the React app
npm run dev
```

The app will be available at `http://localhost:5173` and the API at `http://localhost:3001`.

### 6. Production Build

```bash
npm run build
```

## Deployment

### Vercel Deployment

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Add environment variables in Vercel dashboard:
   - `MONGODB_URI`: Your MongoDB connection string
4. Deploy!

The app includes a `vercel.json` configuration file for seamless deployment.

## API Endpoints

- `POST /api/contact` - Submit contact form
- `GET /api/health` - Health check

## Database Schema

Contact submissions are stored with the following fields:

```javascript
{
  name: String,
  email: String, 
  subject: String,
  message: String,
  timestamp: Date,
  ip: String
}
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).