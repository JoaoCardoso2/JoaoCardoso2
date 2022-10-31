## Olá! eu sou o joão cardoso 2

<div align="center">
  <a href="https://github.com/JoaoCardoso2">
  <img height="200em" src="https://github-readme-stats.vercel.app/api?username=JoaoCardoso2&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
  <img height="128em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JoaoCardoso2&layout=compact&langs_count=7&theme=dracula"/>
</div>

 <div style="display: inline_block"><br>
  <img align="center" alt="joao-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="joao-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="joao-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="joao-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg">
  </div>
  
  ##
  <img align="right" alt="joao-gif" src="https://c.tenor.com/D5QVYSPmpmAAAAAC/anime-keyboard-typing-keyboard-anime.gif">
  
  <div>
<a herf="https://www.instagram.com/cardoso__joao" tagert="_blank"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"
tagert="_blank"></a>
<a herf="https://www.facebook.com/profile.php?id=100008685962448" target="blanc"><img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white"
tagert="_blank"></a>
<a herf="https://wa.me/qr/JM4X5KYYGNFTC1" tagert="_blank"><img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white"
tagert="_blank"></a>
  <div>
    
 ![Snake animation](https://github.com/JoaoCardoso2/JoaoCardoso2/blob/output/github-contribution-grid-snake.svg)

    name: Generate Datas
on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:
jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Summary Cards
      - uses: actions/checkout@v2
      - uses: vn7n24fzkq/github-profile-summary-cards@release
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
        with:
          USERNAME: ${{ github.repository_owner }}

       Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: JoaoCardoso2
          svg_out_path: dist/github-contribution-grid-snake.svg
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
