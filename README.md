# Pioneira Desentupimentos e Caça Vazamentos

Site institucional da Pioneira (desentupimento e caça vazamentos). HTML/CSS/JS estático, sem build.
Mesma estrutura dos outros sites da AROE, com as cores do uniforme da equipe: azul-marinho, dourado
("Desentupimentos") e o azul-água do mascote.

```bash
npx --yes serve . -l 6360
```

## Estrutura

```
index.html
assets/
  css/styles.css
  js/main.js              menu mobile, formulário -> WhatsApp, FAQ, reveal ao rolar, ano do rodapé
  fonts/phosphor/         ícones Phosphor (woff2 local, licença MIT)
  img/
    icon.svg              mascote (gota com lupa) redesenhado em SVG, também é o favicon
    hero.jpg, desentupimento-cozinha.jpg, vazamento-parede.jpg, reparo-tubulacao.jpg, servico-externo.jpg
```

As 5 fotos são **reais**, enviadas pelo cliente (pasta `aroe-sites/pioneira-desentupidora`), redimensionadas
para a web (900 px no hero, 640 px nas demais).

## Dados usados

| Campo | Valor |
|---|---|
| Nome | Pioneira Desentupimentos e Caça Vazamentos (como no uniforme; no Google: "Pioneira Desentupimento e Caça Vazamentos") |
| WhatsApp / telefone | (47) 99292-6875 (`wa.me/5547992926875`) |
| Horário | Fecha às 19h (Google) |
| Google | https://share.google/2ZElGEj7IxpXvu4kd (link no contato e no rodapé) |

**Pedido do cliente: não colocar cidade.** O site não cita cidade, endereço nem mapa (nem nos textos, nem no
SEO/dados estruturados). O formulário pergunta só o bairro. Quem quiser ver a localização tem o link do perfil no
Google.

## Confirmar com o cliente

- **Horário:** o Google só mostra que fecha às 19h. Pegar dias e horário de abertura (e se atende emergência fora
  do horário).
- **Lista de serviços:** desentupimento (pias, ralos, vasos, esgoto, caixa de gordura, cozinhas comerciais) e
  caça vazamentos (ocultos, conta alta, infiltração, troca de tubulação) foram montados a partir das fotos e do
  nome. Confirmar se fazem tudo (ex.: caixa de gordura, hidrojateamento, limpa-fossa).
- **Método de caça vazamentos:** o site diz que localiza o ponto antes de abrir, sem citar equipamento (geofone,
  gás traçador...). Se usarem algum, vale destacar.
- **Logo:** o mascote foi redesenhado em SVG a partir da estampa da camiseta. Pedir a logo original em arquivo.

## Depoimentos

Não foram incluídos (o Google tem só 1 avaliação). Dá para adicionar depois com avaliações reais.

Fontes: Montserrat e Nunito Sans (Google Fonts, OFL).

## Deploy

Sem build: publicar a pasta na Vercel, GitHub Pages ou hospedagem comum.
Depois do deploy, colocar a URL final no `og:image` (precisa ser absoluta) e adicionar `<link rel="canonical">`.
