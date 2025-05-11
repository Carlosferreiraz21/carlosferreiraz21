name: GitHub-Profile-3D-Contrib

on:
  schedule: # 03:00 JST == 18:00 UTC
    - cron: "0 18 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    name: generate-github-profile-3d-contrib
    steps:
      - uses: actions/checkout@v2
      - uses: yoshi389111/github-profile-3d-contrib@0.6.0
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          USERNAME: ${{ github.repository_owner }}
      - name: Commit & Push
        run: |
          git config user.name github-actions
          git config user.email github-actions@github.com
          git add -A .
          git commit -m "generated"
          git push
 👋 Olá, meu nome é Carlos Henrique Ferreira!


Tenho 22 anos, sou Estudante de Análise e Desenvolvimento de Sistemas Ead, concluindo Técnico em Tecnologia da Informação e Comunicação. Pretendo me especializar em IA / Machine Learning / Engenharia de Prompt.
 Ainda não trabalho na área, mas estou me esecializando para isso.

## 🛠️ Tecnologias e Ferramentas

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

## 📬 Entre em contato

📧 Email: carlosferreira.ttech@gmail.com
🔗 [LinkedIn](www.linkedin.com/in/carlos-henrique-ferreira-dev)  

