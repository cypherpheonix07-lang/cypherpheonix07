name: Metrics
on:
  # Schedule daily updates
  schedule: [{cron: "0 0 * * *"}]
  # (Optional) Run workflow manually from the Actions tab
  workflow_dispatch:
  # (Optional) Run on push to the default branch
  push: {branches: ["main", "master"]}
jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - name: Generate metrics image
        uses: lowlighter/metrics@latest
        with:
          token: ${{ secrets.METRICS_TOKEN }}  # store your token as a secret

          # Basic settings
          user: YOUR_GITHUB_USERNAME            # ← replace with your username
          template: classic
          base: header, activity, community, repositories, metadata
          repositories_skipped: YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME  # skip profile repo

          # Plugin: Introduction (like "Joined GitHub ...")
          plugin_introduction: yes
          plugin_introduction_title: yes

          # Plugin: Follow-up (issues and pull requests stats) – optional
          plugin_followup: yes

          # Plugin: Lines of code changed (added/removed)
          plugin_lines: yes

          # Plugin: Habits (coding activity)
          plugin_habits: yes
          plugin_habits_facts: yes
          plugin_habits_charts: yes
          plugin_habits_skipped: YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME

          # Plugin: PageSpeed Insights
          plugin_pagespeed: yes
          plugin_pagespeed_url: https://YOUR_WEBSITE_URL      # ← replace with your site
          plugin_pagespeed_detailed: yes                       # shows scores breakdown

          # Plugin: Calendar (contributions graph)
          plugin_calendar: yes
          plugin_calendar_limit: 1                              # last year

          # Plugin: Commit activity per day (like the "Commits activity per day" chart)
          plugin_activity: yes
          plugin_activity_limit: 10
          plugin_activity_days: 14
          plugin_activity_visibility: all
          plugin_activity_timestamps: yes

          # Plugin: Languages
          plugin_languages: yes
          plugin_languages_ignored: html, css                   # optionally ignore some
          plugin_languages_details: bytes-size, percentage
          plugin_languages_sections: most-used                  # "most used languages" and "language activity"

          # Plugin: Projects (repositories with recent updates)
          plugin_projects: yes
          plugin_proprojects_repositories: YOUR_GITHUB_USERNAME/project1, YOUR_GITHUB_USERNAME/project2   # ← list repos you want to show

          # Plugin: Repositories (like the "Projects" section in your image)
          plugin_repositories: yes
          plugin_repositories_featured: YOUR_GITHUB_USERNAME/repo1, YOUR_GITHUB_USERNAME/repo2   # ← featured repositories

          # Optional: Add a "Contributors" section if needed
          # plugin_contributors: yes
          # plugin_contributors_head: only                    # to show only repository contributors
