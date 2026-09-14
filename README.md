Legal Copilot AI: Enterprise Contract Review Workspace: 
Legal Copilot is a front-end prototype for an enterprise-grade LegalTech application. It demonstrates a complete contract review lifecycle—from intake triage to playbook-driven redlining and final executive sign-off—all running entirely in a single HTML file.
Built with vanilla JavaScript, HTML5, and Tailwind CSS, this zero-build application requires no backend, no dependencies, and runs instantly in any modern web browser.
✨ Core Features & Workflows
1. Dual-Mode Review Workspace
Counsel can toggle instantly between two distinct document reading modes:
Annotated View (Triage & Audit): A structured review canvas where standard text sits in clean boxes, while high-risk clauses are elevated into prominent issue-cards displaying risk severity (High, Medium), playbook explanations, and track-changes redlines.
Clean Parchment View (Continuous Reading): A distraction-free, fluid reading experience styled like traditional legal bond paper (#FCFBF7). Cards and metadata vanish, leaving only subtle in-line highlighter strokes over offending clauses.
2. Multi-Posture AI Redlining & Track Changes
When the system flags a non-compliant clause, counsel can generate dynamic redlines based on three negotiation postures:
Aggressive: Heavily favors the user's corporate position.
Balanced: Standard market language designed for quick mutual agreement.
Minimal: Surgical edits that only fix explicit statutory illegalities.
Once generated, redlines appear as standard legal diffs (~~deleted text~~ and inserted text) that can be accepted or reverted with a single click.
3. Enterprise Clause Repository
A dedicated workspace housing the organization's "Gold Standard" legal language.
Tiered Fallbacks: Clauses are structured by General Counsel preference: Preferred Standard, Fallback A, and Walk-Away Limit.
In-Review "Clause Bank": Counsel can open the repository drawer during a contract review to instantly swap a counterparty's non-compliant text with a pre-approved GC standard.
4. Executive Deal Risk Memorandum
A one-click tool that generates a formal leadership brief summarizing:
The overarching deal risk posture.
Itemized statutory conflicts and financial vulnerabilities.
Actionable negotiation directives.
Export: One-click copy to Markdown for instant sharing via email, Slack, or Jira.
5. Interactive Risk Minimap Rail
A vertical heatmap running along the right edge of the document canvas. Colored ticks indicate the exact scroll position of critical (🔴), medium (🟡), and resolved (🟢) clauses, allowing for rapid navigation through dense agreements.
📂 Preloaded Test Agreements
The application includes four realistic, multi-page commercial contracts preloaded into the queue to demonstrate the AI's auditing capabilities:
Education Loan Sanction Letter (Lumina Education Finance Ltd): Flags illegal compounding penal interest (RBI Fair Lending Code), unconstitutional irrevocable future income assignments, and unilateral change-of-terms clauses.
Enterprise Cloud Master Subscription Agreement (Stratus Cloud Technologies Inc.): Identifies asymmetric liability caps ($10k vendor limit vs. uncapped customer liability) and disclaimers of IP defense obligations.
Commercial Office Lease Agreement (Meridian Commercial Tower Holdings): Audits uncapped controllable Operating Expenses (CAM) and unannounced landlord entry rights.
Senior Secured Credit Facility (Zenith Global Capital Partners): Flags hyper-sensitive $50,000 cross-default thresholds on trade debt.
🚀 Getting Started
This project is entirely self-contained for easy demonstration and prototyping.
Clone or Download the repository to your local machine.
Open dashboard.html in any modern web browser (Chrome, Edge, Safari, Firefox).
No Build Step Required: Tailwind CSS and Phosphor Icons are loaded via CDN. There is no npm install, Webpack, or Node server required.
🛠️ Tech Stack & Architecture
Markup & Styling: HTML5, Tailwind CSS (via CDN)
Icons & Typography: Phosphor Icons, Google Fonts (Inter, Merriweather, JetBrains Mono)
Logic & State: Vanilla JavaScript (ES6). State is managed internally via JavaScript objects representing the mock database of contracts, playbook rules, and repository clauses.
📝 License
This project is intended as a UI/UX prototype and design exploration for enterprise legal technology.
