# Faisal Hossain's Portfolio

Personal portfolio featuring cybersecurity projects, threat research, and data analysis.

Visit the portfolio at [faisalhossainnyc.github.io](https://faisalhossainnyc.github.io/).

## Site content

The home page in `index.html` contains the Projects and Research sections. The site uses Jekyll and is hosted on GitHub Pages. The home page uses a minimal terminal-inspired theme with dark mode by default, an optional light mode, and a saved appearance preference. Theme changes use a short fade and respect reduced-motion preferences.

Reports and their source notebooks are grouped by project under `projects/`. Each project folder contains its readable report, source notebook, and README. Standalone software projects have separate repositories linked from the home page.

## Local development

With Ruby and Bundler installed, run:

```sh
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000` to preview the site. To generate the site without starting a server, run `bundle exec jekyll build`.
