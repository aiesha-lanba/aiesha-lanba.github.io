# Vercel Deployment Guide

This guide will help you deploy the Vendi website to Vercel.

## Prerequisites

1. **GitHub Repository**: Your code should be in a GitHub repository
2. **Vercel Account**: Sign up at [vercel.com](https://vercel.com) using your GitHub account

## Deployment Steps

### Option 1: Deploy via Vercel Dashboard (Recommended)

1. **Connect to Vercel**:
   - Go to [vercel.com](https://vercel.com)
   - Click "Continue with GitHub" to sign in
   - Authorize Vercel to access your GitHub repositories

2. **Import Project**:
   - Click "New Project" or "Add New..."
   - Select "Project" from the dropdown
   - Find your repository `aiesha-lanba.github.io` and click "Import"

3. **Configure Project**:
   - **Project Name**: `vendi-website` (or keep the default)
   - **Framework Preset**: Select "Other" or "Static Site"
   - **Root Directory**: Leave as default (`.`)
   - **Build Command**: Leave empty (static site)
   - **Output Directory**: Leave empty
   - **Install Command**: Leave empty

4. **Deploy**:
   - Click "Deploy"
   - Wait for deployment to complete (usually 1-2 minutes)
   - Your site will be available at `https://your-project-name.vercel.app`

### Option 2: Deploy via Vercel CLI

1. **Install Vercel CLI**:
   ```bash
   npm install -g vercel
   ```

2. **Login to Vercel**:
   ```bash
   vercel login
   ```

3. **Deploy from your project directory**:
   ```bash
   vercel
   ```
   - Follow the prompts
   - Choose "Deploy" when asked

4. **Deploy to Production**:
   ```bash
   vercel --prod
   ```

## Custom Domain (Optional)

1. Go to your project dashboard on Vercel
2. Click on the "Domains" tab
3. Add your custom domain
4. Follow the DNS configuration instructions

## Environment Variables

This project doesn't require any environment variables for basic functionality.

## Automatic Deployments

- Every push to the `main` branch will automatically trigger a new deployment
- Pull requests will create preview deployments
- You can see all deployments in the Vercel dashboard

## Project Structure

The website includes:
- `index.html` - Home page
- `about.html` - About us page
- `software.html` - Software documentation
- `electrical.html` - Electrical documentation
- `mechanical.html` - Mechanical documentation
- `process.html` - Development process
- `gallery.html` - Photo gallery
- `styles.css` - Global styles
- `vercel.json` - Vercel configuration
- `headshotPhotos/` - Team photos and project images

## Features

- Responsive design
- Dark mode theme with red and gold accents
- Animated elements with AOS library
- Photo gallery
- Timeline visualization
- Mobile-friendly navigation

## Support

If you encounter any issues during deployment:
1. Check the Vercel dashboard for build logs
2. Ensure all file paths are correct and case-sensitive
3. Verify that all images exist in the repository
4. Contact Vercel support if needed

## Live URL

Once deployed, your website will be available at:
- Vercel URL: `https://your-project-name.vercel.app`
- Custom domain: (if configured)
