# LearningDayDemoSWA

A simple static "Hello World" web page deployed to Azure Static Web Apps.

## 📁 Project Structure

- `index.html` - Main HTML page with Hello World content
- `staticwebapp.config.json` - Azure Static Web Apps configuration file

## 🚀 Local Development

To view the page locally, simply open `index.html` in your web browser:

```bash
# On Linux/Mac
open index.html

# Or use a simple HTTP server
python -m http.server 8000
# Then visit http://localhost:8000
```

## ☁️ Deploy to Azure Static Web Apps

### Prerequisites
- An Azure account
- Azure Static Web Apps resource

### Deployment Steps

1. **Create Azure Static Web App**:
   - Go to [Azure Portal](https://portal.azure.com)
   - Create a new "Static Web App" resource
   - Connect it to this GitHub repository

2. **Configure Build Settings**:
   - App location: `/` (root directory)
   - Api location: (leave empty)
   - Output location: (leave empty)

3. **Automatic Deployment**:
   - Azure will automatically create a GitHub Actions workflow
   - Every push to the main branch will trigger a deployment
   - The site will be available at the URL provided by Azure

### Manual Deployment using Azure CLI

```bash
# Install Azure Static Web Apps CLI
npm install -g @azure/static-web-apps-cli

# Deploy
swa deploy
```

## 🌐 Features

- ✅ Responsive design
- ✅ Modern styling with gradient backgrounds
- ✅ Smooth animations
- ✅ Azure Static Web Apps configuration
- ✅ SEO-friendly HTML structure

## 📝 Notes

This is a minimal static web application suitable for hosting on Azure Static Web Apps. The `staticwebapp.config.json` file provides configuration for routing and security headers.