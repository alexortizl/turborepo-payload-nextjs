# Turborepo + Payload CMS + Next.js Template

A monorepo starter template that integrates Payload CMS with Next.js applications using Turborepo for efficient build system and project management.

## Features

- 📦 Monorepo setup with Turborepo
- 🚀 Next.js for website projects
- 🎯 Payload CMS as a headless CMS
- 📚 Shared internal library for Payload configuration
- 🔒 Type-safe development experience

## Project Structure

- `apps/payload-admin` - Admin UI for Payload CMS
- `apps/website` - Main Next.js website
- `packages/payload` - Internal library containing Payload CMS configuration and models
- `packages/eslint-config` - Shared ESLint configuration
- `packages/typescript-config` - Shared TypeScript configuration

## Getting Started

1. Clone this repository
2. Install dependencies:
   ```bash
   pnpm install
   ```
3. Set up environment variables:
   - Check `.env.example` files in each project directory
   - Create corresponding `.env` files with your values

### Payload Library

The `packages/payload` directory contains the shared Payload CMS configuration used across projects.

### ESLint Config

The `packages/eslint-config` package provides a consistent linting configuration across all projects in the monorepo.

### TypeScript Config

The `packages/typescript-config` contains shared TypeScript configurations, ensuring consistent type checking and compiler options.

### Payload Admin

The admin interface for managing content is a standalone app located in `apps/payload-admin`, utilizing the shared Payload configuration.

### Web

There is Next.js application located in `apps/website` that consumes content from Payload CMS.
