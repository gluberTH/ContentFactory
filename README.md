# 🚀 Premium AI Content Factory Engine

Welcome to the **Premium AI Content Factory Engine**—a professional, enterprise-grade Python command-line utility built to automatically generate high-converting, SEO-optimized, and industry-grade articles. Designed for content managers, publishers, copywriters, and marketers, this tool automates a rigorous 12-step sequential generation workflow inspired by advanced editorial frameworks.

---

## 🌟 Key Features

- **Automated Idea Brainstorming**: Leverages OpenAI to brainstorm 5 highly engaging, non-cliché topic angles based on your core seed topic.
- **Interactive Terminal Selection**: Pick your target topic directly from an intuitive, interactive console menu.
- **Deep Target Avatar Analysis**: Automatically models a comprehensive psychological profile of your ideal reader, pinpointing their goals, frustrations, fears, and objections.
- **Rigorous Thesis Outlining**: Builds a 5-to-7 section logical article flow (hook, body, practical checklist, high-conversion call-to-action) and details it with 3–5 key arguments per section.
- **Expert-grade Writing style**: Sequentially drafts each article section, naturally embedding real-world analogies, statistics, and highly realistic expert quotes.
- **Semantic LSI Optimization**: Generates a set of 10–15 clustered Latent Semantic Indexing keywords related to your core topic.
- **Deep Editorial Pass**: Runs a final editorial optimization pass to naturally inject keywords, smooth out transitions, and rigorously scrub standard AI clichés (such as *"In today's fast-paced world..."*, *"Moreover"*, *"In conclusion"*).
- **Beautiful Production Outputs**:
  - **Markdown (`.md`)**: A cleanly formatted draft, ready to copy and paste into any CMS or editor.
  - **Premium HTML (`.html`)**: A beautiful, fully styled page featuring a gorgeous, responsive CSS design (complete with Outfit/Inter typography, responsive paddings, dark/light scheme support, styled tables, and custom blockquotes for expert quotes).
- **Smart Spreadsheet Management**:
  - Automatically generates a styled `input.xlsx` template if missing.
  - Automatically appends a comprehensive publishing log row to a persistent `output.xlsx` database on every successful run.

---

## ⚙️ Installation & Setup

This application is designed in modular, lightweight Python. Follow these quick steps to get started:

### 1. Prerequisites
Ensure you have **Python 3.8+** installed on your system. 

### 2. Install Dependencies
Navigate to the tool's directory in your terminal and run:
```bash
pip install -r requirements.txt
```

### 3. Configure API Credentials
1. Copy the `.env.example` file and rename it to `.env`:
   ```bash
   cp .env.example .env
   ```
2. Open the `.env` file in your favorite text editor and paste your OpenAI API Key:
   ```env
   OPENAI_API_KEY=your_actual_openai_api_key_here
   OPENAI_MODEL=gpt-4o
   ```
   > 💡 *Note: We recommend `gpt-4o` for maximum analytical depth and editorial quality, but you can also use `gpt-4o-mini` for highly cost-efficient drafting.*

---

## 📂 Configuration (Input File)

Before running, the tool requires information about your seed topic, audience, and offer. This is managed entirely inside a clean, modern Excel spreadsheet:

When you run the tool for the first time, it will automatically generate a highly styled **`input.xlsx`** file in the root directory. Open it in Microsoft Excel or Google Sheets and configure the following columns:

| Column Header | Description | Example Value |
| :--- | :--- | :--- |
| **Seed Topic/Keyword** | The main topic or core subject of the article. | *Real Estate Investing in Pattaya for Digital Nomads* |
| **Target Audience Brief** | High-level summary of your target reader. | *Young remote workers and digital nomads looking for high passive yield.* |
| **Product/Service Description** | The product or service you want to naturally promote. | *GrandisVillas Premium Rental Management (8% guaranteed ROI).* |
| **Primary SEO Keyword** | The core search term you want to rank for. | *Pattaya property investment digital nomads* |
| **Main Goal** | What you want the reader to do after reading (CTA). | *Book a free Zoom property consultation on our website.* |

Save the spreadsheet. You are now ready to produce content!

---

## 🚀 How to Run

Execute the engine with a single command:
```bash
python content_factory.py
```

### The Generation Workflow:
1. **Init**: The engine reads your variables from `input.xlsx` and initiates a connection to OpenAI.
2. **Concept Selection**: The engine lists 5 highly compelling article ideas in your terminal.
3. **Choice**: Enter `1` to `5` to choose which angle to write.
4. **Drafting**: The engine builds the plan, details it into theses, saves the intermediate plan file to the `output/` folder, and drafts the article section-by-section.
5. **Editorial Pass & Save**: Semantic LSI keywords are generated, injected seamlessly, and final files are saved.

---

## 📈 Outputs

All finished articles are saved directly into the **`output/`** folder:
- **`output/plan_[slug].md`**: The detailed thesis outline for editorial review.
- **`output/[slug].md`**: Polished final article in clean Markdown.
- **`output/[slug].html`**: Premium web article. Double-click to open in any browser or embed directly into your landing page.
- **`output.xlsx`**: A continuous spreadsheet database keeping track of all generated content dates, keywords, paths, and metadata.

---

## 🛡️ License

This product is sold exclusively via Gumroad. Sharing, redistributing, or reselling this source code is strictly prohibited. Thank you for supporting independent creators!
