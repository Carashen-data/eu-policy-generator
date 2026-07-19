# EU Privacy & Cookie Policy Generator

A free, open-source, single-file HTML tool that generates **GDPR** and **ePrivacy Directive** compliant Privacy Policies and Cookie Policies for websites and applications targeting the EU market.

![GDPR](https://img.shields.io/badge/GDPR-Compliant-003399?style=flat-square)
![ePrivacy](https://img.shields.io/badge/ePrivacy-Directive-003399?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

## Live Demo

**[Try it now](https://carashen-data.github.io/eu-policy-generator/)** - No installation required, runs entirely in your browser.

## Features

### Comprehensive Compliance Coverage

Benchmarked against leading EU companies (SAP, Spotify, Klarna) and EDPB/DPA guidance, the generated policies cover:

- **GDPR Articles 5-22, 25-35, 40-49** - Full core compliance
- **ePrivacy Directive Article 5(3)** - Cookie consent requirements
- **EDPB Guidelines** - Transparency, consent, and international transfers
- **CJEU Planet49 ruling** - Cookie consent validity requirements
- **Schrems II** - Transfer Impact Assessments (TIAs)

### Privacy Policy Sections (17 sections)

1. Introduction & legal framework
2. Data Controller & Contacts (including Art. 27 EU Representative)
3. Personal Data categories (16 data types)
4. Special Category Data (Art. 9 - 8 categories)
5. Data Sources (Art. 14 - 7 source types)
6. Purposes & Legal Basis matrix (Spotify-style 3-column table)
7. Legitimate Interest Assessment disclosure
8. Cookies & tracking summary
9. Recipients & data sharing (with sub-processor detail)
10. International transfers (SCCs, BCRs, DPF, TIAs)
11. Data retention (purpose-based with criteria)
12. Data Subject Rights (Art. 15-22 - 9 rights)
13. Security Measures (Art. 32 - 10 measures)
14. Automated Decision-Making & Profiling (Art. 22)
15. Children's Privacy (age-gating, parental consent)
16. Data Protection Governance (DPD, DPIA, ROPA, certifications)
17. Policy changes & contact information

### Cookie Policy Sections (10 sections)

1. Cookie & tracking technology definitions (cookies, beacons, fingerprinting, SDKs)
2. Legal framework (ePrivacy Dir. + GDPR + Planet49)
3. Cookie inventory tables (Name, Provider, Purpose, Type, Duration)
4. 6 cookie categories with detailed per-cookie tables
5. Third-party service registry with privacy links
6. Consent management (CMP provider, renewal period, equal-prominence buttons)
7. Browser management guides
8. Global Privacy Control (GPC) signals
9. Policy updates
10. Contact information

### Generator Features

- **5-step guided form** with progress indicator
- **Real-time preview** of both policies
- **Download as HTML** (print-ready, standalone documents)
- **Copy to clipboard** for quick pasting
- **No server required** - pure client-side HTML/CSS/JS
- **No data leaves your browser** - everything runs locally

## Usage

### Option 1: Online

Visit the [GitHub Pages demo](https://carashen-data.github.io/eu-policy-generator/) - no installation needed.

### Option 2: Local

1. Download `index.html`
2. Open it in any modern web browser
3. Fill in the 5-step form
4. Click "Generate Policies"
5. Preview, download, or copy the output

### Option 3: Self-hosted

```bash
# Clone the repo
git clone https://github.com/Carashen-data/eu-policy-generator.git
cd eu-policy-generator

# Serve with any static server
python3 -m http.server 8080
# or
npx serve .
```

Then open `http://localhost:8080`.

## Technology Stack

- **Pure HTML/CSS/JavaScript** - No frameworks, no build step, no dependencies
- **Single file** (~45KB) - Easy to embed, modify, or self-host
- **Responsive design** - Works on desktop and mobile
- **Print-friendly** - Optimized print stylesheet

## Customization

The generator is a single HTML file. To customize:

- **Branding**: Modify the `.header` CSS section
- **Data categories**: Edit the `DATA_TYPES`, `PURPOSES`, etc. arrays in the `<script>` section
- **Third-party services**: Add/remove entries in the `THIRD_PARTY_SERVICES` array
- **Policy templates**: Modify the `buildPrivacyPolicy()` and `buildCookiePolicy()` functions
- **Labels**: Update the `LABELS` object for policy output text

## Compliance Notes

> **Disclaimer**: This tool generates template policies for reference purposes. It does not constitute legal advice. We strongly recommend having your final policies reviewed by a qualified legal professional to ensure full compliance with applicable EU and national laws.

### Benchmarked Against

| Company | Lessons Applied |
|---------|----------------|
| **SAP** | Purpose-legal basis matrix, email tracking disclosure, EU Cloud CoC, certifications |
| **Spotify** | Named data categories, 3-column purpose matrix, supplementary policies for children |
| **Klarna** | Legitimate interest assessment, automated decision logic disclosure, IMY enforcement lessons |

### DPA Guidance Incorporated

- EDPB Guidelines on consent (05/2020) and transparency (WP260)
- CNIL cookie guidance (13-month renewal, equal-prominence buttons)
- CJEU Planet49 judgment (no pre-ticked boxes, no cookie walls)
- EDPB Recommendations 01/2020 on supplementary measures (Schrems II)

## Contributing

Contributions are welcome! Areas where help is especially appreciated:

- **Multi-language output** - Generate policies in German, French, Spanish, etc.
- **Additional frameworks** - DSA, DMA, AI Act coverage
- **More third-party services** - Expand the service registry
- **Accessibility** - WCAG 2.1 AA compliance
- **PDF export** - In-browser PDF generation

## License

MIT License - see [LICENSE](LICENSE) for details.
