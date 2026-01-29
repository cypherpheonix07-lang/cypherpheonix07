# 🎨 Advanced Customization Guide

## 📊 Stats Card Customization

### Available Themes
```markdown
# Dark Themes
- dark
- radical
- merko
- gruvbox
- tokyonight
- onedark
- cobalt
- synthwave
- highcontrast
- dracula

# Light Themes
- default
- graywhite
- vue
- buefy

# Special Themes
- github_dark
- nord
- monokai
```

### Custom Colors
```markdown
![Stats](https://github-readme-stats.vercel.app/api?username=USERNAME&bg_color=0d1117&title_color=58a6ff&text_color=c9d1d9&icon_color=58a6ff&border_color=30363d)
```

### Hide Specific Stats
```markdown
![Stats](https://github-readme-stats.vercel.app/api?username=USERNAME&hide=stars,commits,prs,issues&show_icons=true)
```

### Show All Stats
```markdown
![Stats](https://github-readme-stats.vercel.app/api?username=USERNAME&show_icons=true&include_all_commits=true&count_private=true)
```

---

## 💻 Language Stats Options

### Compact Layout
```markdown
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=USERNAME&layout=compact)
```

### Hide Specific Languages
```markdown
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=USERNAME&hide=html,css)
```

### Show More Languages
```markdown
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=USERNAME&langs_count=10)
```

### Custom Card Width
```markdown
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=USERNAME&card_width=445)
```

---

## 🔥 Streak Stats Customization

### Basic Streak
```markdown
![Streak](https://github-readme-streak-stats.herokuapp.com/?user=USERNAME)
```

### Custom Colors
```markdown
![Streak](https://github-readme-streak-stats.herokuapp.com/?user=USERNAME&theme=dark&hide_border=true&background=0d1117&stroke=58a6ff&ring=58a6ff&fire=ff6b6b&currStreakLabel=58a6ff)
```

### Available Streak Themes
- default
- dark
- highcontrast
- radical
- merko
- gruvbox
- tokyonight
- onedark
- cobalt
- synthwave
- dracula
- prussian
- monokai
- vue
- vue-dark
- shades-of-purple
- nightowl
- buefy
- blue-green
- algolia
- great-gatsby
- darcula
- bear
- solarized-dark
- solarized-light
- chartreuse-dark
- nord
- gotham
- material-palenight
- graywhite
- vision-friendly-dark
- ayu-mirage
- midnight-purple
- calm
- flag-india
- omni
- react
- jolly
- maroongold
- yeblu
- blueberry
- slateorange
- kacho_ga

---

## 🏆 Trophy Customization

### Basic Trophy
```markdown
![Trophy](https://github-profile-trophy.vercel.app/?username=USERNAME)
```

### Themes
```markdown
# Available themes: flat, onedark, gruvbox, dracula, monokai, chalk, nord, alduin, darkhub, juicyfresh, buddhism, oldie, radical, onestar, discord, algolia, gitdimmed, tokyonight, matrix, apprentice, dark_dimmed, dark_lover

![Trophy](https://github-profile-trophy.vercel.app/?username=USERNAME&theme=darkhub&no-frame=true&no-bg=true&margin-w=4)
```

### Hide Specific Trophies
```markdown
![Trophy](https://github-profile-trophy.vercel.app/?username=USERNAME&no-frame=true&no-bg=true&margin-w=4&column=7&rank=-C,-B)
```

---

## 🎵 Music Integration Examples

### Spotify - Currently Playing
```markdown
[![Spotify](https://novatorem-USERNAME.vercel.app/api/spotify)](https://open.spotify.com/user/USERNAME)
```

### Spotify - Recently Played
```markdown
[![Spotify](https://spotify-github-profile.vercel.app/api/view?uid=SPOTIFY_ID&cover_image=true&theme=default)](https://spotify-link-to-submit.vercel.app/)
```

### Apple Music
```markdown
[![Apple Music](https://music-profile.rayriffy.com/theme/dark.svg?uid=APPLE_MUSIC_ID)](https://music.apple.com/profile/USERNAME)
```

### Last.fm - Recent Tracks
```markdown
![Last.fm](https://lastfm-recently-played.vercel.app/api?user=LASTFM_USERNAME&count=5)
```

---

## 📈 Activity Graph Options

### Basic Graph
```markdown
![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=USERNAME)
```

### Themed Graph
```markdown
![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=USERNAME&theme=github-dark&hide_border=true&bg_color=0d1117&color=58a6ff&line=58a6ff&point=ff6b6b)
```

### Available Themes
- default
- github
- github-dark
- github-light
- xcode
- rogue
- merko
- vue
- tokyo-night
- high-contrast
- dracula
- gruvbox
- chartreuse-dark
- react-dark

---

## 🎯 Badges and Icons

### Skill Icons
```markdown
# Simple Icons
![Skills](https://skillicons.dev/icons?i=js,ts,react,nodejs,python,docker)

# Themed Icons
![Skills](https://skillicons.dev/icons?i=js,ts,react,nodejs,python,docker&theme=dark)

# Custom Perline
![Skills](https://skillicons.dev/icons?i=js,ts,react,nodejs,python,docker&perline=3)
```

### Tech Stack Badges
```markdown
# Style Options: flat, flat-square, plastic, for-the-badge, social

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
```

### Dynamic Badges
```markdown
# Followers
![Followers](https://img.shields.io/github/followers/USERNAME?style=for-the-badge)

# Stars
![Stars](https://img.shields.io/github/stars/USERNAME?style=for-the-badge)

# Profile Views
![Views](https://komarev.com/ghpvc/?username=USERNAME&style=for-the-badge)
```

---

## 🐍 Snake Animation Options

### Color Customization
In your `snake.yml` workflow:

```yaml
- name: Generate Snake
  uses: Platane/snk/svg-only@v3
  with:
    github_user_name: ${{ github.repository_owner }}
    outputs: |
      dist/github-contribution-grid-snake.svg
      dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9
      dist/rainbow.gif?color_snake=blue&color_dots=red,orange,yellow,green,blue
```

---

## 📊 WakaTime Integration

### Setup
1. Install WakaTime in your code editor
2. Get your API key from [WakaTime Dashboard](https://wakatime.com/settings/account)
3. Add to README:

```markdown
![WakaTime Stats](https://github-readme-stats.vercel.app/api/wakatime?username=WAKATIME_USERNAME&layout=compact&theme=dark)
```

### Detailed Stats
```markdown
![WakaTime](https://wakatime.com/share/@USERNAME/WAKATIME_EMBED_ID.svg)
```

---

## 🎭 Profile Views Counter

### Simple Counter
```markdown
![Profile Views](https://komarev.com/ghpvc/?username=USERNAME)
```

### Styled Counter
```markdown
![Profile Views](https://komarev.com/ghpvc/?username=USERNAME&color=blueviolet&style=for-the-badge&label=PROFILE+VIEWS)
```

### Counter Colors
- brightgreen
- green
- yellow
- yellowgreen
- orange
- red
- blue
- grey
- lightgrey
- blueviolet
- ff69b4 (custom hex)

---

## 🌟 GitHub Skyline

Generate a 3D model of your GitHub contributions:
```markdown
![GitHub Skyline](https://skyline.github.com/USERNAME/2024.png)
```

---

## 📱 Social Media Badges

### LinkedIn
```markdown
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/USERNAME)
```

### Twitter/X
```markdown
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/USERNAME)
```

### Instagram
```markdown
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/USERNAME)
```

### YouTube
```markdown
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@USERNAME)
```

### Discord
```markdown
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/INVITE)
```

### Website/Portfolio
```markdown
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=react&logoColor=white)](https://yourwebsite.com)
```

---

## 🎨 Custom Sections

### Add a Quote
```markdown
<div align="center">
  
  ### 💡 Quote of the Day
  
  ![Quote](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=dark)
  
</div>
```

### Random Dev Joke
```markdown
![Jokes Card](https://readme-jokes.vercel.app/api?theme=dark)
```

### Typing SVG
```markdown
[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=58A6FF&center=true&vCenter=true&width=435&lines=Full+Stack+Developer;Open+Source+Contributor;Tech+Enthusiast)](https://git.io/typing-svg)
```

---

## 🔧 Advanced Tips

### 1. Use HTML for Better Control
```html
<div align="center">
  <img src="URL" width="400" alt="Description">
</div>
```

### 2. Create Collapsible Sections
```markdown
<details>
<summary>Click to expand!</summary>

### Hidden Content
This content is initially hidden.

</details>
```

### 3. Add Horizontal Rules
```markdown
---
or
***
or
___
```

### 4. Center Everything
```html
<div align="center">
  <!-- Your content here -->
</div>
```

### 5. Add Tables
```markdown
| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Data 1   | Data 2   | Data 3   |
```

---

## 🚀 Performance Optimization

1. **Limit the number of widgets** - Too many can slow loading
2. **Use caching** - Most services cache results automatically
3. **Optimize images** - Compress profile pictures
4. **Use SVG when possible** - They load faster than PNG/JPG
5. **Test on mobile** - Ensure responsive design

---

## 📝 Markdown Tips

### Text Formatting
```markdown
**Bold Text**
*Italic Text*
***Bold and Italic***
~~Strikethrough~~
`Code`
```

### Links
```markdown
[Link Text](URL)
[Link with Title](URL "Title")
```

### Images
```markdown
![Alt Text](URL)
![Alt Text](URL "Title")
```

### Lists
```markdown
- Item 1
- Item 2
  - Nested Item

1. First
2. Second
3. Third
```

### Code Blocks
````markdown
```language
code here
```
````

---

## 🎯 Examples of Great Profiles

Check these profiles for inspiration:
- [abhisheknaiidu](https://github.com/abhisheknaiidu)
- [anuraghazra](https://github.com/anuraghazra)
- [DenverCoder1](https://github.com/DenverCoder1)
- [rafaballerini](https://github.com/rafaballerini)

---

## 📚 Additional Resources

- [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [GitHub Profile README Generator](https://rahuldkjain.github.io/gh-profile-readme-generator/)
- [Markdown Guide](https://www.markdownguide.org/)
- [Shields.io](https://shields.io/)
- [Simple Icons](https://simpleicons.org/)

---

**Happy Customizing! 🎉**
