# Arpan Guria - Production Level Portfolio

This is a production-ready portfolio website for Arpan Guria with a Node.js Express backend, Firebase Realtime Database for data storage, and Cloudinary for image management.

## Features

- Admin panel for content management
- Image carousel management with Cloudinary
- Case studies and portfolio projects
- Firebase Realtime Database for data persistence
- JWT-based authentication
- RESTful API endpoints for portfolio items, case studies, and content sections

## Getting Started

### Prerequisites

- Node.js 14+
- npm or yarn
- Firebase project
- Cloudinary account

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/Mapileon2/Arpan-Guria-Production-level-Portfolio.git
cd Arpan-Guria-Production-level-Portfolio
```

2. **Install dependencies**

```bash
npm install
```

3. **Configure Environment Variables**

Create a `backend.env` file in the root directory with the following variables (see backend.env.example):

```
JWT_SECRET=your_jwt_secret_here

# Firebase Configuration
FIREBASE_TYPE=service_account
FIREBASE_PROJECT_ID=your-project-id
FIREBASE_PRIVATE_KEY_ID=your_private_key_id_here
FIREBASE_PRIVATE_KEY="-----BEGIN PRIVATE KEY-----\nYOUR_PRIVATE_KEY_HERE\n-----END PRIVATE KEY-----\n"
FIREBASE_CLIENT_EMAIL=your_client_email_here
FIREBASE_CLIENT_ID=your_client_id_here
FIREBASE_DATABASE_URL=https://your-project-id-default-rtdb.firebaseio.com

# Cloudinary Configuration
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

4. **Start the development server**

```bash
node server.js
```

The server will start on port 5000 (or the port specified in your environment variables).

## Vercel Deployment

This project is configured for deployment on Vercel:

1. Push the code to GitHub
2. Import the repository in Vercel
3. Configure the environment variables in Vercel
4. Deploy

## API Endpoints

### Public Endpoints

- `GET /api/projects` - Get all projects
- `GET /api/case-studies` - Get all case studies
- `GET /api/case-studies/:id` - Get a single case study
- `GET /api/carousel-images` - Get carousel images
- `GET /api/carousel-settings` - Get carousel settings

### Admin Endpoints

- `POST /api/case-studies` - Create a new case study
- `PUT /api/case-studies/:id` - Update a case study
- `DELETE /api/case-studies/:id` - Delete a case study
- `POST /api/carousel-images` - Add a carousel image
- `PUT /api/carousel-images/:id` - Update a carousel image
- `DELETE /api/carousel-images/:id` - Delete a carousel image
- `POST /api/upload` - Upload an image

## Admin Panel

Access the admin panel at `/admin.html`. For development, you can use the direct login page at `/direct-login.html`.

## License

MIT 
#   A r p a n - G u r i a - P r o d u c t i o n - l e v e l - P o r t f o l i o 
 
 