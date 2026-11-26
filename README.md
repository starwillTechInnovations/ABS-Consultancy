# M S Kadam & Associates — Chartered Accountants Official Web Platform

A complete, modern, professional, and fully responsive Chartered Accountancy firm website inspired by and benchmarked against [M S Kadam & Associates](https://www.mskadamandassociates.com/).

Built with **React.js**, **Vite**, **Tailwind CSS**, **Lucide React**, **React Hook Form**, and **Zod**, with full architectural preparation for **Python FastAPI** and **PostgreSQL** backend integration.

---

## 🏛️ Firm Overview & Practice Standards
* **Firm Name:** M S Kadam & Associates (Chartered Accountants)
* **Accreditation:** Registered with the Institute of Chartered Accountants of India (ICAI), Peer-Reviewed Practice
* **Managing Partner:** CA M. S. Kadam (B.Com, FCA)
* **Head Office:** Office No. 70, 4th Floor, Patil Arcade, Above Kalinga Hotel, Khilare Road, Near Tech Mahindra, Erandwane, Pune - 411004, Maharashtra
* **Contact:** +91 9028644499 | rahulchate.ca@gmail.com
* **Core Philosophy:** *Professional Expertise. Practical Solutions. Reliable Advisory.*

---

## 🚀 Key Features

### 1. Corporate & Trust-First Design
- **Institutional Palette:** Deep Corporate Navy (`#0F172A`, `#1E293B`) paired with Warm Gold/Amber accents (`#D97706`) and neutral slates.
- **ICAI Compliance Disclaimer:** Mandatory regulatory notification in full compliance with the Institute of Chartered Accountants of India code of ethics.
- **Mobile Responsive:** Seamless experience across mobile smartphones, tablets, laptops, and ultra-wide desktops.

### 2. Comprehensive Practice Verticals (10 Specialized Areas)
1. **GST Services:** GSTR-1, 3B, 9/9C, ITC 2B reconciliations, and inverted duty refunds.
2. **Income Tax Services:** Corporate/Individual ITR, faceless scrutiny defense, and NRI Form 15CA/15CB.
3. **Tax Audit:** Section 44AB audits, Form 3CA/3CB/3CD, and depreciation schedules.
4. **Statutory Audit:** Companies Act 2013 audit, CARO 2020 reporting, and true-and-fair view assurance.
5. **Internal Audit:** Internal Financial Controls (IFC) testing, SOP reviews, and leakage mitigation.
6. **Accounting & Bookkeeping:** Cloud accounting (Tally Prime, Zoho Books, QuickBooks) and monthly MIS dashboards.
7. **Company Registration:** Turnkey MCA SPICe+ incorporation of Private Limited, LLPs, and Section 8 companies.
8. **Corporate Compliance:** Annual ROC filings (AOC-4, MGT-7), DIR-3 KYC, and secretarial documentation.
9. **Financial Advisory & Virtual CFO:** Rolling cash flow models, unit economics, and board financial stewardship.
10. **Business Consulting:** Entity restructuring, DCF/NAV business valuations, and M&A due diligence.

### 3. Sector-Specific Compliance Frameworks (8 Industries)
- Manufacturing & Engineering (AS-2 / Ind AS 2 inventory, inverted duty refunds)
- IT, Software & SaaS (Ind AS 115 revenue recognition, zero-rated export LUT)
- Startups & Emerging Ventures (DPIIT recognition, Section 80-IAC, cap-table advisory)
- Real Estate & Construction (RERA CA certifications, JDA Section 45(5A) taxation)
- Healthcare & Pharma (Exempt healthcare vs taxable medicines, machinery depreciation)
- Retail & E-commerce (Marketplace TCS reconciliations, multi-state GST)
- Agriculture & Agro-Processing (Agricultural income vs food processing, FPO governance)
- NGOs, Trusts & Section 8 (Section 12AB/80G renewals, FCRA compliances)

### 4. Interactive Financial Calculators Suite
- **Income Tax Calculator:** Dynamic comparison of **Old vs. New Tax Regime (Section 115BAC)** under the latest FY 2024-25 provisions, including the revised ₹75,000 standard deduction, Section 87A rebates, Chapter VI-A deductions (80C, 80D, 80CCD(1B) NPS), and Section 24(b) home loan interest.
- **GST Forward & Reverse Calculator:** Calculates base value, CGST, SGST, and gross total across 5%, 12%, 18%, and 28% tax slabs.
- **HRA Exemption Calculator:** Computes Section 10(13A) deductions for metro (50%) and non-metro (40%) cities.
- **NPS Retirement Calculator:** Projects compound corpus growth and ₹50,000 additional Section 80CCD(1B) tax savings.
- **Gratuity Benefit Calculator:** Computes statutory gratuity entitlement under the 15/26 formula and Section 10(10) ₹20 Lakh exemption cap.
- **Statutory Tax Due Date Calendar:** Recurring monthly, quarterly advance tax, and annual filing deadlines.

### 5. Conversion & Engagement Utilities
- **Dual-Mode Consultation Form:** Validated via **Zod** and **React Hook Form**, supporting both in-person Pune office visits and virtual Google Meet/Zoom consultations.
- **Floating WhatsApp Quick-Action:** Direct pre-filled WhatsApp chat link to `+91 9028644499`.
- **TopBar:** Quick access to contact numbers, email, Pune location, and tax calendar.

---

## 🛠️ Technology Stack

| Layer | Tools & Libraries |
| :--- | :--- |
| **Framework** | React 18 with Vite 6 |
| **Styling** | Tailwind CSS v3 with PostCSS and Autoprefixer |
| **Routing** | React Router DOM v6 with ScrollToTop restoration |
| **Icons** | Lucide React |
| **Form Handling** | React Hook Form |
| **Validation** | Zod + `@hookform/resolvers` |
| **HTTP Client** | Axios (with environment variable support) |
| **Backend-Ready** | Python FastAPI & PostgreSQL endpoint blueprints |

---

## 📁 Project Architecture

```
msk-accounting-website/
│
├── public/
│   ├── images/
│   ├── logo.png
│   └── favicon.ico
│
├── src/
│   ├── assets/
│   │
│   ├── components/
│   │   ├── TopBar.jsx            # Top info bar (phone, email, hours, tax calendar link)
│   │   ├── Navbar.jsx            # Sticky responsive nav with services dropdown & mobile drawer
│   │   ├── HeroSection.jsx       # 2-column hero with corporate snapshot card
│   │   ├── TrustIndicators.jsx   # 4 core trust pillars (ICAI standards, UDIN, ethics)
│   │   ├── ServiceCard.jsx       # Reusable service card with icons & features
│   │   ├── ServicesSection.jsx   # Homepage services grid with category filters
│   │   ├── WhyChooseUs.jsx       # 6 core competencies & client benefits
│   │   ├── IndustryCard.jsx      # Reusable industry vertical card
│   │   ├── IndustriesSection.jsx # 8-industry showcase
│   │   ├── IndustryDetails.jsx   # Detailed challenges and CA solutions view
│   │   ├── TaxCalculator.jsx     # Old vs New Regime interactive calculator component
│   │   ├── WorkflowSection.jsx   # 4-step client engagement timeline (desktop/mobile)
│   │   ├── Testimonials.jsx      # Client feedback carousel (sample case studies)
│   │   ├── ConsultationForm.jsx  # Zod-validated consultation inquiry form
│   │   ├── Footer.jsx            # Multi-column footer with ICAI disclaimer
│   │   └── WhatsAppButton.jsx    # Persistent floating WhatsApp quick action
│   │
│   ├── pages/
│   │   ├── Home.jsx              # Comprehensive landing page
│   │   ├── About.jsx             # Firm story, values, vision/mission, leadership
│   │   ├── Services.jsx          # All 10 services with full scope and FAQs
│   │   ├── Industries.jsx        # Detailed sector solutions & challenges
│   │   ├── Calculators.jsx       # 5 calculators + statutory tax calendar dashboard
│   │   ├── Contact.jsx           # Office details, Google Maps, enquiry form
│   │   └── PrivacyPolicy.jsx     # ICAI Code of Ethics data protection policy
│   │
│   ├── data/
│   │   ├── services.json         # Static data for 10 practice verticals with FAQs
│   │   ├── industries.json       # Sector-specific challenges & CA solutions
│   │   └── testimonials.json     # Client feedback data
│   │
│   ├── hooks/
│   │   └── useTaxCalculator.js   # Dynamic tax calculation logic (FY 2024-25)
│   │
│   ├── services/
│   │   └── api.js                # Axios client prepared for FastAPI endpoints
│   │
│   ├── App.jsx                   # Root router configuration
│   ├── main.jsx                  # React DOM root entry
│   └── index.css                 # Tailwind directives & base styles
│
├── .env                          # Local environment variables
├── .env.example                  # Environment configuration template
├── .gitignore                    # Git exclusions
├── package.json                  # Dependencies and scripts
└── README.md                     # Documentation
```

---

## ⚡ Getting Started & Execution

### Prerequisites
- **Node.js**: v18.0.0 or higher (Tested on Node v24.20.0)
- **npm**: v9.0.0 or higher

### 1. Installation
Clone or navigate to the project directory:
```bash
cd "ABS consultancy"
npm install
```

### 2. Environment Setup
Verify or customize `.env`:
```env
VITE_API_BASE_URL=http://localhost:8000/api
VITE_APP_TITLE=M S Kadam & Associates - Chartered Accountants
VITE_OFFICE_PHONE=+91 9028644499
VITE_OFFICE_EMAIL=rahulchate.ca@gmail.com
VITE_WHATSAPP_NUMBER=919028644499
```

### 3. Run Development Server
```bash
npm run dev
```
The application will launch at `http://localhost:3000` (or `http://localhost:5173`).

### 4. Production Build
```bash
npm run build
```
Generates production-optimized static assets in the `/dist` directory.

### 5. Preview Production Build
```bash
npm run preview
```

---

## 🔌 Future Backend Integration (FastAPI & PostgreSQL)

The frontend is built with `src/services/api.js`, pre-configured to communicate with the following FastAPI endpoints:

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/api/services` | Fetches active practice verticals & service FAQs |
| `GET` | `/api/industries` | Fetches sector-specific challenges & solutions |
| `GET` | `/api/testimonials`| Fetches verified client testimonials |
| `POST` | `/api/contact` | Submits client consultation requests to PostgreSQL |
| `POST` | `/api/calculator` | Server-side tax simulation & logging |
| `POST` | `/api/admin/login` | JWT authentication for firm partners |
| `GET` | `/api/admin/leads` | Partner dashboard to review incoming enquiries |

When the FastAPI server is running, the frontend seamlessly connects without component alterations. If the backend is offline, the frontend falls back gracefully to structured local data without breaking or showing simulated false successes.

---

## ⚖️ Legal & Professional Notice
*This software implementation is inspired by the web design and practice areas of M S Kadam & Associates (Chartered Accountants, Pune) for client advisory and business consultancy web deployment.*
#   A B S - C o n s u l t a n c y  
 