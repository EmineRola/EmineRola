        Hi Im Emine 👋
- ❔ I am a front-end React developer and special education teacher.
- 🌱 I transfer what I learned during the education process to my projects in the most professional way.
- 👯 I am highly motivated, organized, and I can work well, both independently and as part of a team.
- ⚡ I am open to learning and I follow new technologies closely.
 
                                                             Visitors  -   Tech Stack                                                           
                               
  <p align="center">
      <img height="180em" src="https://github-readme-stats.vercel.app/api?username=EmineRola&theme=blue-green&show_icons=true&count_private=true)"/>
      <img height="180em" src="https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=EmineRola&layout=compact&langs_count=8&theme=blue-green"/>
</p>
 name: Generate Snake

on:
  schedule:
    - cron: "0 */6 * * *"

  workflow_dispatch:


jobs:
  build:
    runs-on: ubuntu-latest
    steps:

      - uses: actions/checkout@v2

      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: EmineRola
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg

      - run: git status

      - name: Push changes
        uses: ad-m/github-push-action@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          branch: master
          force: true

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 



   socials
   
   [![Instagram Badge](https://img.shields.io/badge/-Instagram-C13584?style=flat-quare&labelColor=C13584&logo=instagram&logoColor=white&link=link)]([link](https://www.instagram.com/emine_gucluerr/?igshid=YWJhMjlhZTc%3D)) 
   
  

   
   
    
    
   
