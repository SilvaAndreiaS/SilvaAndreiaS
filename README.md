### Hello My Name Andreia Souza 👋

[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/andreiasouzasantana/)[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SilvaAndreiaS)[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/an.dreiasou?igsh=MW5vc3N1cXRsaWFvcQ%3D%3D&utm_source=qr)[![Android Developers](https://img.shields.io/badge/Android-Developers-brightgreen)](https://developer.android.com/)[![Google Developers - Andreia Souza](https://img.shields.io/badge/Google%20Developers-Andreia%20Souza-blue?logo=google)](https://g.dev/AndreiaSouzaS)

## Tecnologias Que  Utilizo 



<div style="display: inline_block"><br/>
<img align="center" alt="Sass" src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white"/>
<img align="center" alt="C++" src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white"/>
<img align="center" alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
<img align="center" alt="Kotlin" src="https://img.shields.io/badge/Kotlin-0095D5?&style=for-the-badge&logo=kotlin&logoColor=white"/>
<img align="center" alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img align="center" alt="JavaScript" src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E"/>
<img align="center" alt="HTML" src="https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white"/>
</div>



# Tecnologias Que Utilizo

<div style="display: inline_block"><br/>
<img align="center" alt="Sass" src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white"/>
<img align="center" alt="C++" src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white"/>
<img align="center" alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
<img align="center" alt="Kotlin" src="https://img.shields.io/badge/Kotlin-0095D5?&style=for-the-badge&logo=kotlin&logoColor=white"/>
<img align="center" alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img align="center" alt="JavaScript" src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E"/>
<img align="center" alt="HTML" src="https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white"/>
</div>

# Redes Sociais

[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/an.dreiasou?igsh=MW5vc3N1cXRsaWFvcQ%3D%3D&utm_source=qr)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SilvaAndreiaS)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/andreiasouzasantana/)

# Animação

![snake gif](https://github.com/SilvaAndreiaS/SilvaAndreiaS/blob/output/github-contribution-grid-snake.svg)

name: Generate Snake Animation

on:
  schedule: # execute every 12 hours
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout the repository
        uses: actions/checkout@v2

      - name: Generate snake animation
        uses: Platane/snk@master
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          output: "github-contribution-grid-snake.svg"

      - name: Commit and push if changes are made
        run: |
          git config --global user.name 'github-actions[bot]'
          git config --global user.email '41898282+github-actions[bot]@users.noreply.github.com'
          git add github-contribution-grid-snake.svg
          git commit -m "Generated snake animation"
          git push
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

