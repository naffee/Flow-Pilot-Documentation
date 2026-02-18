# FlowPilot Knowledgebase

![Build Status](https://img.shields.io/badge/build-passing-brightgreen) ![Jekyll](https://img.shields.io/badge/jekyll-4.3-blue) ![Just the Docs](https://img.shields.io/badge/theme-just--the--docs-success)

Official documentation and help center for **FlowPilot**, the AI-powered workflow automation platform. This repository contains the source code for the static site generated with Jekyll.

## 🚀 Features

- **Modern SaaS Design:** Clean, responsive UI with custom typography and color palette.
- **Search Enabled:** Built-in search functionality for quick access to topics.
- **Structured Content:** Organized into Getting Started, Features, Troubleshooting, and FAQs.
- **Easy Deployment:** Static site architecture ready for GitHub Pages or Netlify.

## 🛠 Tech Stack

- **Generator:** [Jekyll](https://jekyllrb.com/)
- **Theme:** [Just the Docs](https://just-the-docs.github.io/just-the-docs/)
- **Styling:** SCSS (Sass)
- **Language:** Markdown / Liquid

## 📦 Installation & Setup

### Prerequisites

Ensure you have the following installed:
- [Ruby](https://rubyinstaller.org/) (v2.7+)
- [Bundler](https://bundler.io/) (`gem install bundler`)

### Local Development

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/flowpilot-docs.git
   cd flowpilot-docs
   ```

2. **Install dependencies:**
   ```bash
   bundle install
   ```
   *(Note: If on Windows, ensure you have the Ruby DevKit installed)*

3. **Run the server:**
   ```bash
   bundle exec jekyll serve
   ```

4. **View the site:**
   Open your browser to `http://localhost:4000`

## 📂 Project Structure

```text
FlowPilot/
├── _config.yml               # Site configuration (title, theme settings)
├── Gemfile                   # Ruby dependencies
├── index.md                  # Homepage
├── assets/
│   └── css/                  # Styling entry point
├── _sass/                    # Custom SCSS overrides
│   └── custom_style.scss     
└── docs/                     # Documentation Content
    ├── getting-started/
    ├── features/
    ├── account/
    ├── troubleshooting/
    └── faq/
```

## 🎨 Customization

### Styling
Custom styles are located in `_sass/custom_style.scss`. This file overrides the default theme variables and adds specific SaaS-style refinements.

### Configuration
Edit `_config.yml` to change the site title, description, color scheme, or navigation settings.

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
