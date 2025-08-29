# Vercel Deployment Guide

This project is configured for deployment on Vercel. Due to the Arabic characters and spaces in the current folder path, you may encounter build issues locally.

## Quick Deployment Steps

### Option 1: Direct Vercel Deployment (Recommended)
1. Push your code to a GitHub repository
2. Connect your GitHub repository to Vercel
3. Vercel will automatically detect the Vite framework and deploy
4. The `vercel.json` configuration file is already set up

### Option 2: Vercel CLI Deployment
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in the project directory
3. Follow the prompts to deploy

## Configuration Files

- `vercel.json`: Deployment configuration
- `vite.config.ts`: Build configuration with proper base path
- `package.json`: Contains build scripts

## Build Configuration

The project includes:
- Framework detection for Vite
- Proper output directory (`dist`)
- SPA routing configuration
- Build optimization settings

## Environment Variables

If you need environment variables:
1. Add them to your Vercel project settings
2. They will be automatically available during build

## Troubleshooting

If you encounter path-related build issues:
1. Copy the project to a folder with English-only characters
2. Or deploy directly from a Git repository (recommended)

## Live URL

After deployment, your presentation will be available at:
`https://your-project-name.vercel.app`