# MAP=MeauxbilityAdminPortal

# 🏢 Meauxbility Foundation - Corporate Monorepo

> # 🏢 Meauxbility Foundation - Corporate Monorepo

> **Next-generation operations platform for accessibility, innovation, and social impact**

[![Live Admin Portal](https://img.shields.io/badge/Live-Admin%20Portal-00D4AA?style=for-the-badge&logo=vercel)](https://iaudodidact.com/)
[![Next.js](https://img.shields.io/badge/Next.js-14-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase)](https://supabase.com/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel)](https://vercel.com/)

---

## 🎯 Corporate Overview

**Meauxbility Foundation** is a technology-driven nonprofit focused on accessibility, innovation, and social impact. Our corporate monorepo houses all digital infrastructure, applications, and tools that power our mission.

### 🌐 Live Properties
- **Admin Portal:** [iaudodidact.com](https://iaudodidact.com/) - Operations dashboard
- **Nonprofit Site:** [meauxbility.org](https://meauxbility.org) - Public website (migrating to Vercel)
- **E-commerce:** [inneranimals.com](https://inneranimals.com) - Online store (migrating to Vercel)
- **Additional Domain:** [meauxxx.com](https://meauxxx.com) - Reserved for future use

### 🏗️ Past Builds & Portfolio
- **Spartans Command Center:** [inneranimal.github.io/spartans_command_center/](https://inneranimal.github.io/spartans_command_center/) - Meauxbility TRUTEC Stack showcase - https://inneranimal.github.io/fred/ ( best version so far of accurate meauxbility.org brand lol) 
- **Swampblood.com** - Planned rebuild (repository pending)
- **Fuelnfreetime.com** - Planned rebuild (repository pending)
-Adelyn Cook Consulting - marketing application
-Blair Mann - Mann Enterprise - c-corp - repo pending
-Southern Pets Animal Rescue - repo pending
-MsHippi.com - repo pending
---

## 🏗️ Monorepo Structure

```
meauxbilityfoundation/.org/
├── 📱 apps/
│   ├── admin-portal/          # Next.js 14 admin dashboard (LIVE)
│   ├── meauxbility-org/       # Nonprofit website (MIGRATING)
│   ├── inneranimals-shop/     # E-commerce platform (MIGRATING)
│   ├── spartans-command-center/ # TRUTEC Stack showcase (LIVE)
│   ├── swampblood/            # Planned rebuild (PENDING)
│   ├── fuelnfreetime/         # Planned rebuild (PENDING)
│   └── api-gateway/           # Centralized API services (PLANNED)
├── 🛠️ packages/
│   ├── ui-components/         # Shared React components
│   ├── database-schemas/      # Supabase migrations
│   ├── auth-system/           # Authentication & RBAC
│   ├── asset-manager/         # Google Drive + Cloudflare R2
│   └── ai-integrations/       # OpenAI, Claude, Analytics
├── 🔧 tools/
│   ├── deployment/            # Vercel configs
│   ├── monitoring/            # Performance tracking
│   └── automation/            # CI/CD scripts
└── 📚 docs/
    ├── api-documentation/     # API references
    ├── deployment-guides/     # Setup instructions
    └── corporate-policies/    # Governance docs
```

---

## 🚀 Current Status

### ✅ Production Ready
- **Admin Portal** - Live at [iaudodidact.com](https://iaudodidact.com/)
  - Next.js 14 with App Router
  - Supabase backend (PostgreSQL, Auth, Real-time)
  - 7 functional modules (GitHub, Brand Lab, Analytics, etc.)
  - Role-based access control (Admin, CTO, CMO, Members)
  - Secure API routes for external integrations

### 🔄 In Migration
- **meauxbility.org** - Moving from Render to Vercel
- **inneranimals.com** - Moving from current host to Vercel
- **Asset Management** - Google Drive + Cloudflare R2 integration

### 🔄 Planned Rebuilds
- **swampblood.com** - Rebuilding with modern stack (Next.js, Supabase)
- **fuelnfreetime.com** - Rebuilding with modern stack (Next.js, Supabase)

### 📋 Planned
- **AI-Powered Workflows** - OpenAI + Claude integration
- **Advanced Analytics** - Google Analytics + custom metrics
- **Payment Processing** - Stripe integration
- **Team Collaboration** - Real-time features

---

## 🛠️ Technology Stack

### Frontend
- **Next.js 14** (App Router, Server Components)
- **React 19** (Latest features)
- **Tailwind CSS** (Utility-first styling)
- **Lucide Icons** (Icon system)

### Backend
- **Supabase** (PostgreSQL, Auth, Storage, Real-time)
- **Row Level Security** (Data protection)
- **API Routes** (Secure server-side operations)

### External Services
- **GitHub API** (Repository management)
- **Google Drive API** (Asset management)
- **Cloudflare R2** (CDN + Storage)
- **OpenAI API** (AI content generation)
- **Claude API** (Advanced AI analysis)
- **Google Analytics** (Performance tracking)
- **Stripe API** (Payment processing)

### Deployment
- **Vercel** (Hosting platform)
- **Custom Domains** (iaudodidact.com, meauxbility.org, inneranimals.com)
- **SSL/HTTPS** (Secure connections)

---

## 👥 Team Structure

### Leadership
- **Sam** (CEO) - `sam@meauxbility.org` - Full admin access
- **Fred Williams** (CMO) - `fred@meauxbility.org` - Marketing & campaigns
- **Connor McNeely** (CTO) - `connor@meauxbility.org` - Technical operations

### Access Levels
- **Admin** - Full system access, user management, API keys
- **CTO** - Technical operations, GitHub integration, deployments
- **CMO** - Marketing tools, campaigns, analytics
- **Members** - Basic access, content creation

---

## 🔑 Environment Variables

### Required for All Apps
```bash
# Supabase (Core Backend)
NEXT_PUBLIC_SUPABASE_URL=...
NEXT_PUBLIC_SUPABASE_ANON_KEY=...
SUPABASE_SERVICE_ROLE=...

# GitHub Integration
GITHUB_TOKEN=...

# AI Services
OPENAI_API_KEY=...
ANTHROPIC_API_KEY=...

# Google Services
GOOGLE_CLIENT_ID=...
GOOGLE_CLIENT_SECRET=...
NEXT_PUBLIC_GA_MEASUREMENT_ID=...

# Cloudflare R2 (Asset Storage)
CLOUDFLARE_ACCOUNT_ID=...
CLOUDFLARE_ACCESS_KEY_ID=...
CLOUDFLARE_SECRET_ACCESS_KEY=...
CLOUDFLARE_R2_BUCKET=meauxbility-assets
CLOUDFLARE_R2_PUBLIC_URL=https://assets.iaudodidact.com

# Stripe (Payments)
STRIPE_PUBLISHABLE_KEY=...
STRIPE_SECRET_KEY=...
```

---

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- Git
- Vercel CLI (optional)
- Supabase account

### Development Setup
```bash
# Clone repository
git clone https://github.com/meauxbilityfoundation/.org.git
cd .org

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Edit .env.local with your keys

# Start development server
npm run dev

# Visit http://localhost:3000
```

### Production Deployment
```bash
# Deploy to Vercel
vercel --prod

# Or push to main branch (auto-deploys)
git add .
git commit -m "Deploy to production"
git push origin main
```

---

## 📱 Applications

### 1. Admin Portal (`/apps/admin-portal`)
**Live:** [iaudodidact.com](https://iaudodidact.com/)

**Features:**
- 7 functional modules (GitHub, Brand Lab, Analytics, Campaigns, Grants, Website Builder, Settings)
- Command palette (⌘K) for quick navigation
- Real-time collaboration
- Role-based access control
- Secure API integrations

**Tech:** Next.js 14, Supabase, Tailwind CSS

### 2. Meauxbility.org (`/apps/meauxbility-org`)
**Status:** Migrating to Vercel

**Purpose:** Public nonprofit website
- Mission and impact stories
- Donation processing
- Volunteer opportunities
- Accessibility resources
- Grant application system

### 3. Inner Animals Shop (`/apps/inneranimals-shop`)
**Status:** Migrating to Vercel

**Purpose:** E-commerce platform
- Product catalog
- Shopping cart
- Payment processing (Stripe)
- Order management

### 4. Spartans Command Center (`/apps/spartans-command-center`)
**Status:** Live on GitHub Pages

**Purpose:** Meauxbility TRUTEC Stack showcase
- Technology stack demonstration
- Grant statistics (50+ grants, $250K+ distributed)
- 501(c)(3) nonprofit information
- Acadiana region coverage

**Live:** [inneranimal.github.io/spartans_command_center/](https://inneranimal.github.io/spartans_command_center/)

### 5. Swampblood.com (`/apps/swampblood`)
**Status:** Planned rebuild

**Purpose:** TBD (repository pending)
- Modern Next.js architecture
- Supabase backend
- Integrated with corporate monorepo

### 6. Fuelnfreetime.com (`/apps/fuelnfreetime`)
**Status:** Planned rebuild

**Purpose:** TBD (repository pending)
- Modern Next.js architecture
- Supabase backend
- Integrated with corporate monorepo

---

## 🔧 Development Workflow

### Branch Strategy
- `main` - Production-ready code
- `develop` - Integration branch
- `feature/*` - Feature development
- `hotfix/*` - Critical fixes

### Code Standards
- **ESLint** - Code linting
- **Prettier** - Code formatting
- **TypeScript** - Type safety (planned)
- **Conventional Commits** - Commit messages

### Testing
- **Unit Tests** - Component testing
- **Integration Tests** - API testing
- **E2E Tests** - User flow testing (planned)

---

## 📊 Monitoring & Analytics

### Performance Tracking
- **Vercel Analytics** - Core Web Vitals
- **Google Analytics** - User behavior
- **Custom Metrics** - Business KPIs

### Error Monitoring
- **Vercel Error Tracking** - Runtime errors
- **Supabase Logs** - Database issues
- **Custom Alerts** - Critical failures

---

## 🔒 Security

### Data Protection
- **Row Level Security** (RLS) in Supabase
- **API Key Encryption** - Stored securely
- **OAuth 2.0** - Secure authentication
- **HTTPS Everywhere** - Encrypted connections

### Access Control
- **Role-based permissions** - Granular access
- **API rate limiting** - Abuse prevention
- **Input validation** - XSS protection
- **CORS configuration** - Cross-origin security

---

## 📚 Documentation

### API Documentation
- [Admin Portal API](./docs/api-documentation/admin-portal.md)
- [Supabase Schema](./docs/api-documentation/supabase-schema.md)
- [External Integrations](./docs/api-documentation/external-apis.md)

### Deployment Guides
- [Vercel Setup](./docs/deployment-guides/vercel-setup.md)
- [Environment Variables](./docs/deployment-guides/environment-variables.md)
- [Domain Configuration](./docs/deployment-guides/domains.md)

### Corporate Policies
- [Code of Conduct](./docs/corporate-policies/code-of-conduct.md)
- [Security Guidelines](./docs/corporate-policies/security.md)
- [Access Control](./docs/corporate-policies/access-control.md)

---

## 🤝 Contributing

### For Team Members
1. **Fork** the repository
2. **Create** a feature branch
3. **Make** your changes
4. **Test** thoroughly
5. **Submit** a pull request

### For External Contributors
1. **Read** our Code of Conduct
2. **Check** open issues
3. **Fork** and contribute
4. **Follow** our coding standards

---

## 📞 Support

### Technical Issues
- **GitHub Issues** - Bug reports and feature requests
- **Slack** - Team communication
- **Email** - `tech@meauxbility.org`

### Business Inquiries
- **Email** - `info@meauxbility.org`
- **Website** - [meauxbility.org](https://meauxbility.org)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🎯 Mission Statement

**Meauxbility Foundation** is committed to creating accessible, innovative technology solutions that empower individuals and communities. Through our corporate monorepo, we maintain the highest standards of code quality, security, and user experience while advancing our mission of social impact through technology.

### 📊 Impact Metrics
- **50+ Grants Awarded** - Supporting spinal cord injury survivors
- **$250K+ Funds Distributed** - Adaptive equipment and accessibility services
- **100% Acadiana Coverage** - Serving Louisiana's Acadiana region
- **24/7 Support Available** - Continuous assistance for our community

### 🏛️ Legal Status
- **501(c)(3) Nonprofit** - Tax-exempt charitable organization
- **EIN:** 33-4214907
- **Location:** Lafayette, Louisiana (Acadiana Region)

---

**Built with ❤️ by the Meauxbility Foundation Team**

## 👥 Team

- **Sam** - CEO/Founder (Admin)
- **Connor McNeely** - CTO
- **Fred Williams** - CMO

## 🆘 Support

For issues or questions:

- Create an issue in this repository
- Contact: sam@meauxbility.org
- Slack: #admin-portal

---

Built with 💜 for accessibility and impact

