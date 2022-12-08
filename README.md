
## Oiii eu sou a Samantha Ferreira!
<div align="center">
  <a href="https://github.com/sammyferreira">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=sammyferreira&show_icons=true&theme=dracula&include_all_commits=true&count_private=true"/>
  <img height="100em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=sammyferreira&layout=compact&langs_count=7&theme=dracula"/>
</div>
<div style="display: inline_block"><br>
  <img align="center" alt="Sammy-Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="Sammy-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="Sammy-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="Sammy-Python" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
  <img align="center" alt="Sammy-Csharp" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg">
  <img align="right" alt="Sammy-pic" height="150" style="border-radius:50px;" 
</div>
  
  ##
 
<div> 
  <a href="https://instagram.com/saah18_" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a href = "mailto:samanthafsf1995@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/Samantha Ferreira" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
 
  ![Snake animation](https://github.com/sammyferreira/sammyferreira/blob/output/github-contribution-grid-snake.svg)
 
</div>
  
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
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: SammyFerreira
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
