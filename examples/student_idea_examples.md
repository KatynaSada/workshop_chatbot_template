# Workshop chatbot idea examples

Adapt each idea to your own organization.

Write your config files and `company_data/` content **in English**.

---

## Banking, financial services and financial retail

**Sector context:** organizations with many repeated queries, regulation and a need for traceability.

- **Bot goal:** answer frequent customer questions (products, hours, channels) and know when to escalate to a human.
- **What to put in `company_data/`:** product FAQ, service channel guide, glossary of terms, summary of public policies (non-sensitive information only).
- **Recommended tools:** `search_company_data`, `current_datetime`, `create_support_ticket`

**Internal variant:** employee assistant for commercial onboarding processes or compliance checklists (fictional data).

---

## Technology and digital transformation

**Sector context:** teams integrating systems, documenting APIs and automating workflows.

- **Bot goal:** help staff look up internal documentation, explain deployment processes or answer questions about a digital product/service.
- **What to put in `company_data/`:** project README, architecture guide, technical FAQ, endpoint table (fictional), best-practices manual.
- **Recommended tools:** `search_company_data`, `calculator` (capacity/cost estimates), `current_datetime`

**Agent variant:** bot that combines doc search + calculator to estimate sprint times or resources (sample data).

---

## Education, training and entrepreneurship

**Sector context:** universities, training centres and entrepreneurship programmes.

- **Bot goal:** guide students or teachers (calendar, procedures, resources, campus or programme FAQs).
- **What to put in `company_data/`:** student guide, academic calendar, enrolment FAQ, library resources, campus use rules (public or fictional).
- **Recommended tools:** `search_company_data`, `current_datetime`

**Teacher variant:** assistant that summarises a long document in `company_data/` and answers in a pedagogical tone (adjust `personality.json`).

---

## Marketing and media

**Sector context:** campaign, research and content teams.

- **Bot goal:** explain agency/department services, help locate briefs, templates or brand guidelines (fictional or public data).
- **What to put in `company_data/`:** brand tone guide, services FAQ, target audience examples, campaign checklist, metrics glossary.
- **Recommended tools:** `search_company_data`, `calculator` (simple budgets or KPIs)

**Creative variant:** bot that suggests campaign ideas **only** from uploaded documents (rule in `personality.json`: do not invent client data).

---

## Infrastructure, logistics and operations

**Sector context:** field operations, terminals, maintenance and critical processes.

- **Bot goal:** support teams with procedures, checklists and resolution of common incidents.
- **What to put in `company_data/`:** operations manual, alarm code table, safety procedure, shift FAQ, escalation contacts (fictional).
- **Recommended tools:** `search_company_data`, `calculator`, `create_support_ticket`, `current_datetime`

**Maintenance variant:** bot for technicians that searches PDF manuals and estimates times or consumption with the calculator.

---

## Retail, fashion, small business and consulting

**Sector context:** sales, customer service and admin tasks with limited resources.

- **Bot goal:** inform about products/services, hours, shipping, appointments or consulting packages.
- **What to put in `company_data/`:** catalogue in CSV/TXT, returns policy, pricing, commercial FAQ, professional services description.
- **Recommended tools:** `search_company_data`, `calculator`, `create_support_ticket`

**Consulting variant:** bot that explains methodology and project types from a dossier in `company_data/`, without giving real legal or tax advice.

---

## Choose your idea in 5 minutes

1. Pick a **sector** (above) and a **target user** (external customer vs internal employee).
2. Write **one sentence** for the goal in `config/company.json` → `bot_goal`.
3. Upload at least **2–3 files** to `company_data/`.
4. Choose **2–3 tools** and leave one disabled so you can compare behaviour in the workshop.
5. Adjust **tone** in `config/personality.json` to match the sector (more formal for banking, warmer for retail/education).

**Workshop rule:** public or fictional data only. Never real customer information, accounts, passwords or personal data.
