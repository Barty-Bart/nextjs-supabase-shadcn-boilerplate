# Next.js + Supabase + shadcn/ui Boilerplate

A minimal, production-ready starter template for building internal tools and web apps.

## Features

- ✅ **Next.js 16** - App Router, React Server Components
- ✅ **Supabase** - Auth, database, storage
- ✅ **shadcn/ui** - Beautiful, accessible UI components
- ✅ **Tailwind CSS** - Utility-first styling
- ✅ **TypeScript** - Type safety
- ✅ **Collapsible Sidebar** - Ready-to-use dashboard layout
- ✅ **Auth flows** - Login, logout working

## Prerequisites

- Node.js 20+ (`node -v` to check)
- A Supabase account ([supabase.com](https://supabase.com))

## Quick Start

1. **Clone the repo**
```bash
   git clone https://github.com/Barty-Bart/nextjs-supabase-shadcn-boilerplate.git
   cd nextjs-supabase-shadcn-boilerplate
```

2. **Install dependencies**
```bash
   npm install
```

3. **Set up environment variables**
```bash
   cp .env.example .env.local
```
   
   Then edit `.env.local` with your Supabase credentials:
```
   NEXT_PUBLIC_SUPABASE_URL=https://your-project.supabase.co
   NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=your-anon-key
```
   
   Get these from: Supabase Dashboard → Project Settings → API

4. **Run the dev server**
```bash
   npm run dev
```

5. **Open http://localhost:3000**

## Project Structure
```
app/
  page.tsx              → Redirects to login or dashboard
  auth/                 → Login, signup, password reset
  dashboard/            → Protected dashboard page
    layout.tsx          → Sidebar layout
    page.tsx            → Dashboard content
components/
  app-sidebar.tsx       → Sidebar with navigation
  ui/                   → shadcn components
lib/
  supabase/             → Supabase client setup
  utils.ts              → Utility functions
```

## Adding shadcn Components
```bash
npx shadcn@latest add [component-name]
```

Browse components: https://ui.shadcn.com/docs/components

## Customization

- **Sidebar menu items**: Edit `components/app-sidebar.tsx`
- **Theme/colors**: Edit `app/globals.css`
- **Auth redirects**: Edit `components/login-form.tsx`

## License

MIT
