# Krisleitometro

Medidor oficial do dia: aperte o botão e descubra se hoje você está mais pra **Krisleite** (0) ou pra **Tifanometro** (100). O ponteiro gira, para num número aleatório e aparece um polaroid com um GIF de meme de gato ou cachorro e uma frase sobre o seu resultado.

É um site estático: um único `index.html`, sem build, sem dependências.

## Rodar no computador

Abra o `index.html` direto no navegador. Os GIFs vêm da internet, então precisa estar online.

## Como colaborar

1. Faça um fork e crie uma branch (`git switch -c minha-ideia`).
2. Edite o `index.html`.
3. Abra um pull request contando o que mudou.

Os lugares mais fáceis de mexer ficam no começo do `<script>`:

- **`FAIXAS`**: as faixas do medidor (até qual número vai cada uma), a cor de cada faixa e as frases sorteadas. Para criar frase nova é só adicionar uma linha na `lista` da faixa.
- **`GATOS`** e **`CACHORROS`**: os IDs dos GIFs do GIPHY. O ID é o final do link do GIF, por exemplo em `giphy.com/gifs/cat-meme-Cm4ZDVRSsr7pHbNmKM` o ID é `Cm4ZDVRSsr7pHbNmKM`. Use só GIFs de gato ou cachorro com classificação livre.

Cores e fontes ficam nas variáveis do `:root`, no começo do `<style>`.

## Publicar

Qualquer hospedagem de site estático serve (GitHub Pages, Vercel, Netlify). No GitHub Pages: Settings > Pages > Deploy from a branch > `main` / raiz.

## Créditos

GIFs via [GIPHY](https://giphy.com). Os direitos de cada GIF são dos seus autores.
