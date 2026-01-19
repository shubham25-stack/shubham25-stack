<br clear="both">

<h1 align="center">Hey 👋What's Up?</h1>

###

<div align="center">
  <img src="https://skillicons.dev/icons?i=js" height="60" alt="javascript logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=ts" height="60" alt="typescript logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=nextjs" height="60" alt="nextjs logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=tailwind" height="60" alt="tailwindcss logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="60" alt="react logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" height="60" alt="nodejs logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=express" height="60" alt="express logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" height="60" alt="cplusplus logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" height="60" alt="mongodb logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=postgres" height="60" alt="postgresql logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=prisma" height="60" alt="prisma logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=py" height="60" alt="python logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=aws" height="60" alt="amazonwebservices logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/googlecloud/googlecloud-original.svg" height="60" alt="googlecloud logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=docker" height="60" alt="docker logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=kubernetes" height="60" alt="kubernetes logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=jenkins" height="60" alt="jenkins logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=git" height="60" alt="git logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=postman" height="60" alt="postman logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=linux" height="60" alt="linux logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=vscode" height="60" alt="vscode logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=autocad" height="60" alt="autocad logo"  />
</div>

###

<div align="center">
  <a href="https://www.linkedin.com/in/shubham-thakur-0b281524b/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="linkedin logo"  />
  </a>
  <img src="https://img.shields.io/static/v1?message=Twitter&logo=twitter&label=&color=1DA1F2&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="twitter logo"  />
  <img src="https://img.shields.io/static/v1?message=Discord&logo=discord&label=&color=7289DA&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="discord logo"  />
  <a href="shubham.codecreator@gmail.com" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Gmail&logo=gmail&label=&color=D14836&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="gmail logo"  />
  </a>
</div>

###

<br clear="both">

<div align="center">
  <img src="https://streak-stats.demolab.com?user=shubham25-stack&locale=en&mode=daily&theme=dracula&hide_border=false&border_radius=5&order=3" height="150" alt="streak graph"  />
  <img src="https://github-profile-trophy.vercel.app?username=shubham25-stack&theme=dracula&column=-1&row=1&margin-w=8&margin-h=8&no-bg=false&no-frame=false&order=4" height="150" alt="trophy graph"  />
</div>

###

<br clear="both">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/shubham25-stack/shubham25-stack/output/pacman-contribution-graph-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/shubham25-stack/shubham25-stack/output/pacman-contribution-graph.svg">
  <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/shubham25-stack/shubham25-stack/output/pacman-contribution-graph.svg">
</picture>

###

<img src="https://raw.githubusercontent.com/shubham25-stack/shubham25-stack/output/snake.svg" alt="Snake animation" />

###
name: Generate snake animation

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"

  workflow_dispatch:

  push:
    branches:
    - main

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      - name: generate snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: dist/snake.svg?palette=github-dark


      - name: push snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

###

<div align="center" style="width: 100%">
  <a target="_blank" href="https://github-readme-medium-recent-article.vercel.app/medium/@undefined/0">
    <img style="width: 100%" src="https://github-readme-medium-recent-article.vercel.app/medium/@undefined/0" alt="Medium post 1"  />
  </a>
  <a target="_blank" href="https://github-readme-medium-recent-article.vercel.app/medium/@undefined/1">
    <img style="width: 100%" src="https://github-readme-medium-recent-article.vercel.app/medium/@undefined/1" alt="Medium post 2"  />
  </a>
  <a target="_blank" href="https://github-readme-medium-recent-article.vercel.app/medium/@undefined/2">
    <img style="width: 100%" src="https://github-readme-medium-recent-article.vercel.app/medium/@undefined/2" alt="Medium post 3"  />
  </a>
</div>

###
