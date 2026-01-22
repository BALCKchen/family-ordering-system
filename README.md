# 家庭订购系统 (Family Ordering System)

A Next.js-based family ordering system with Vercel Speed Insights integration for performance monitoring.

## Features

- Built with **Next.js 16** using the App Router
- TypeScript for type safety
- Tailwind CSS for styling
- ESLint for code quality
- **Vercel Speed Insights** for performance monitoring

## Getting Started

### Prerequisites

- Node.js (v18 or higher recommended)
- npm, yarn, pnpm, or bun package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/BALCKchen/family-ordering-system.git
cd family-ordering-system
```

2. Install dependencies:
```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

3. Run the development server:
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### Build for Production

```bash
npm run build
npm start
```

### Linting

```bash
npm run lint
```

## Vercel Speed Insights Integration

This project includes **Vercel Speed Insights** for monitoring and analyzing web performance metrics in production.

### What is Speed Insights?

Vercel Speed Insights helps you understand your application's real-world performance by collecting and analyzing Core Web Vitals and other important metrics directly from user browsers.

### How It Works

The `SpeedInsights` component from `@vercel/speed-insights/next` has been integrated into the root layout (`app/layout.tsx`). This component:

1. Automatically tracks performance metrics
2. Sends anonymized data to Vercel (only when deployed to Vercel)
3. Provides insights into real user experience

### Configuration

#### Enable Speed Insights on Vercel

To enable Speed Insights metrics collection:

1. Go to your [Vercel Dashboard](https://vercel.com/dashboard)
2. Select your project
3. Navigate to the **Speed Insights** tab
4. Click **Enable**

Once enabled, the tracking routes will be available at `/_vercel/speed-insights/*` after your next deployment.

#### View Metrics

After deployment to Vercel and once you have user traffic:

1. Navigate to your project's **Speed Insights** tab in the Vercel Dashboard
2. View real-time performance metrics and trends
3. Analyze Core Web Vitals:
   - Largest Contentful Paint (LCP)
   - First Input Delay (FID)
   - Cumulative Layout Shift (CLS)

### Privacy & Data Compliance

Vercel Speed Insights is designed with privacy in mind:
- Metrics are collected in an anonymized manner
- No personally identifiable information is transmitted
- Data retention follows GDPR and other compliance standards
- Users can opt-out through browser privacy settings

For more details, see [Vercel Speed Insights Privacy Policy](https://vercel.com/docs/speed-insights/privacy-policy).

## Project Structure

```
.
├── app/
│   ├── layout.tsx       # Root layout with SpeedInsights component
│   ├── page.tsx         # Home page
│   └── globals.css      # Global styles
├── public/              # Static assets
├── package.json         # Dependencies and scripts
├── tsconfig.json        # TypeScript configuration
├── tailwind.config.ts   # Tailwind CSS configuration
└── eslint.config.mjs    # ESLint configuration
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run lint` - Run ESLint

## Deployment

### Deploy to Vercel

The easiest way to deploy this Next.js app is using [Vercel Platform](https://vercel.com):

1. Push your code to GitHub, GitLab, or Bitbucket
2. Import the repository into Vercel
3. Configure environment variables if needed
4. Deploy!

### Enable Speed Insights After Deployment

1. Open your Vercel project dashboard
2. Go to the **Speed Insights** tab
3. Click **Enable** to start collecting performance metrics

Metrics will begin appearing in your dashboard once users start visiting your site.

## Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [Vercel Speed Insights Documentation](https://vercel.com/docs/speed-insights)
- [Vercel Speed Insights Getting Started](https://vercel.com/docs/speed-insights/getting-started)
- [Core Web Vitals Guide](https://web.dev/vitals/)
- [Tailwind CSS Documentation](https://tailwindcss.com)

## License

This project is open source and available under the MIT License.

## Support

For issues and feature requests, please visit the [GitHub repository](https://github.com/BALCKchen/family-ordering-system).
