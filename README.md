# CxSE Platform

CXS Enablement - AI-powered sales, onboarding, and support training platform.

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- MongoDB Atlas account
- OpenAI API key
- Vercel account (for deployment)

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/cxse-platform.git
   cd cxse-platform
   ```

2. **Install dependencies**
   ```bash
   npm run install-all
   ```

3. **Environment Setup**
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

4. **Start development servers**
   ```bash
   npm run dev
   ```

### 🚀 Vercel Deployment

1. **Connect to Vercel**
   - Push your code to GitHub
   - Connect your GitHub repository to Vercel
   - Vercel will automatically detect the configuration

2. **Environment Variables**
   Set these in Vercel dashboard:
   ```
   MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/cxse
   JWT_SECRET=your-super-secret-jwt-key
   OPENAI_API_KEY=your-openai-api-key
   NODE_ENV=production
   ```

3. **MongoDB Atlas Setup**
   - Create a MongoDB Atlas cluster
   - Whitelist Vercel IPs (0.0.0.0/0 for development)
   - Create a database user
   - Get connection string

### �� Configuration

#### Required Environment Variables
- `MONGODB_URI` - MongoDB connection string
- `JWT_SECRET` - Secret for JWT token signing
- `OPENAI_API_KEY` - OpenAI API key for AI features

#### Optional Environment Variables
- `SMTP_HOST` - Email server for invitations
- `SMTP_USER` - Email username
- `SMTP_PASS` - Email password
- `VERCEL_URL` - Vercel deployment URL

### 📁 Project Structure
