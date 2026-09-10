# CamJobs V4 🇨🇲
This is the V4 real-platform foundation: Vite frontend + Supabase Auth + Postgres + Row Level Security.

Setup:
1. Create a Supabase project.
2. Run `supabase/schema.sql` in SQL Editor.
3. Copy `.env.example` to `.env` and add your project URL and anon key.
4. Run `npm install` and `npm run dev`.
5. Build with `npm run build` and deploy the frontend to Netlify.
6. Add the same VITE variables in Netlify environment settings.

Admin:
Create the admin user in Supabase Auth, then use the SQL comment at the bottom of schema.sql to assign role=admin. Do not put the admin password in frontend code.

Current V4 includes real authentication, persistent users, job posting, job search, applications, dashboards, saved_jobs schema, and RLS.
Production next: CV uploads, password reset, admin moderation UI, email verification UX, stronger validation/rate limiting, audit logs, monitoring, and payments/featured jobs.