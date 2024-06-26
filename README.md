# GitHub Action for generating a contribution graph with a snake eating your contributions.

name: Generate Snake

# Controls when the action will run. This action runs every 6 hours.

on:
  schedule:
      # every 6 hours
    - cron: "0 */6 * * *"

# This command allows us to run the Action automatically from the Actions tab.
  workflow_dispatch:

# The sequence of runs in this workflow:
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:

    # Checks repo under $GITHUB_WORKSHOP, so your job can access it
      - uses: actions/checkout@v2

    # Generates the snake  
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: mishmanners
          # these next 2 lines generate the files on a branch called "output". This keeps the main branch from cluttering up.
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg

     # show the status of the build. Makes it easier for debugging (if there's any issues).
      - run: git status

      # Push the changes
      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          # the output branch we mentioned above
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Kanit&weight=600&size=30&pause=1000&random=false&width=435&lines=%F0%9F%98%8E+MD+H+R+ALIF)](https://git.io/typing-svg)

**`A passionate (Web Developer/Game Developer/Graphics & ui-ux Designer)`**

<div align="left"> 
  <a href=" https://mail.google.com/mail/u/?authuser=hasiburrahman999.alif@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-333333?style=for-the-badge&logo=gmail&logoColor=red" />
  </a>
  <a href="https://www.linkedin.com/in/md-h-r-alif-7358801a6/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank" />
  </a>
  <a href="https://mdhralif.github.io/portfolio/" target="_blank">
     <img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=todoist&logoColor=white" target="_blank" />
  </a>
</div>



### 🧰 Languages and Tools

<img align="left" alt="Java" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg"/>
<img align="left" alt="Spring" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" />
<img align="left" alt="TypeScript" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-plain.svg" />
<img align="left" alt="Angular" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-plain.svg" />
<img align="left" alt="Git" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" />
<img align="left" alt="Linux" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" />
<img align="left" alt="HTML" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain.svg" />
<img align="left" alt="CSS" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain.svg" />
<img align="left" alt="JavaScript" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" />
<img align="left" alt="React" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" />
<img align="left" alt="NodeJS" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" />
<img align="left" alt="Python" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-plain.svg" />
<img align="left" alt="C++" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-line.svg" />
<img align="left" alt="GitHub" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" />
<img align="left" alt="Bash" width="30px" style="padding-right:10px;" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/bash/bash-original.svg" />
<br />

#



### 📺 Latest Projects

<img align="left" alt="Java" width="232px" style="padding-right:10px;" src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/NexTalk.png"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/bus.png"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/fight.jpg"/>


<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>

<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>
<img align="left" alt="Java" width="232px" style="padding-right:10px; " src="https://raw.githubusercontent.com/mdhralif/portfolio/main/calculator.jpg"/>
<br />

#


### 📊 Stats

![mdhralif's GitHub stats](https://github-readme-stats.vercel.app/api?username=mdhralif&show_icons=true&theme=gruvbox)

<!-- ![GitHub Streak](https://streak-stats.demolab.com?user=ForrestKnight&theme=gruvbox&border_radius=4.5) -->

#

<div align="center">
  <h2>🐍 My Contributions 🐍</h2>
  <br>
  <img alt="snake eating my contributions" src="https://raw.githubusercontent.com/mdhralif/mdhralif/output/github-contribution-grid-snake.svg" />
  
  <br/><br/><br/>
</div>

<hr/>

<h2 align="center">⚡ Stats ⚡</h2>
<br>
<div align=center>
  <img width=390 src="https://github-readme-streak-stats-salesp07.vercel.app/?user=salesp07&count_private=true&theme=react&border_radius=10" alt="streak stats"/>
  <img width=390 src="https://github-readme-stats-salesp07.vercel.app/api?username=salesp07&count_private=true&show_icons=true&theme=react&rank_icon=github&border_radius=10" alt="readme stats" />
  <br/>
  <img width=325 align="center" src="https://github-readme-stats-salesp07.vercel.app/api/top-langs/?username=salesp07&hide=HTML&langs_count=8&layout=compact&theme=react&border_radius=10&size_weight=0.5&count_weight=0.5&exclude_repo=github-readme-stats" alt="top langs" />
</div>

<br/><br/>

<hr/>

<br/>








