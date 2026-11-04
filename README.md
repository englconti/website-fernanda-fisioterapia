# Éfis Terapias | Dra. Fernanda Costa

Site de uma página para a clínica de fisioterapia e terapias integrativas da Dra. Fernanda Costa, na Lagoa da Conceição, em Florianópolis (SC). Feito só com HTML e CSS, sem JavaScript.

## Como ver

Abra o `index.html` no navegador. Para testar com um servidor local:

```bash
python3 -m http.server 8000
```

Depois acesse http://localhost:8000.

## Estrutura

```
index.html          página única
css/styles.css      todo o estilo, com as cores e fontes em :root
assets/img/         fotos usadas no site (WebP, 800 px de largura)
assets/favicon.svg  ícone da aba (flor de lótus)
reference_images/   fotos originais enviadas como referência (não são usadas direto pelo site)
```

## Dados da clínica (do Google Maps)

- Nome no Google: Dra. Fernanda Costa - Éfis terapias (fisioterapeuta)
- Bairro: Lagoa da Conceição (confirmado pela dona; o Google Maps mostra Retiro).
- Endereço: Av. Prefeito Acácio Garibaldi, nº 174, Lagoa da Conceição, Florianópolis - SC, 88062-600
- Coordenadas: -27.6105375, -48.4423141
- Telefone: (48) 99194-8152
- Nota: 5,0 com 75 avaliações
- Serviços na faixada: Fisioterapia, Fonoaudiologia, Terapias Integrativas, Pilates e Massoterapia
- Atendimento com horário marcado

## Decisões de design

- **Cores:** papel lilás-claro `#FBF7FC`, lilás da faixada `#C48ED8`, verde-água do logotipo `#2E9C8F` (`#17766B` nos botões, para contraste) e berinjela escura `#241B2D` no texto e nas faixas escuras.
- **Fontes:** Marcellus nos títulos e Figtree no texto (Google Fonts).
- **Motivo da marca:** a "pétala", com cantos opostos arredondados nas fotos, vem da flor de lótus do logotipo.
- **Serviços:** painéis com as fotos do espaço. No desktop, o painel sob o mouse (ou com foco do teclado) se abre. No celular, todos aparecem empilhados.
- **Movimento:** só um, a pétala da foto principal se abrindo ao carregar. Respeita `prefers-reduced-motion`.

## Confirmado

- Atendimento de segunda a sexta, das 8h às 20h.
- O (48) 99194-8152 é também o WhatsApp da clínica.
- Fotos de pacientes e depoimentos liberados para uso.

## Pendências para confirmar

- Se a fonoaudiologia é atendida na clínica e qual texto usar. Esse painel está sem foto.
- Biografia, formação e número do CREFITO da Dra. Fernanda.
- Se o logotipo pode ser substituído pelo arquivo original (o do site é um desenho simplificado da flor de lótus).
- Endereço do site e imagem de compartilhamento (`og:image`), quando houver domínio.
- Texto do painel "Constelação sistêmica" (é provisório) e confirmar o nome do serviço.
- Foto da fonoaudiologia (painel segue sem foto).
- Sobram em `reference_images/` as fotos 010 (fachada alternativa), 014 (sala de pilates) e 015 (cartas sobre a mesa).

## Design (versão modernizada)

- **Tipografia:** Fraunces (títulos, serifa suave) e Figtree (texto), hospedadas em `assets/fonts/` (licenças OFL incluídas). Nenhuma requisição a Google Fonts.
- **Cores:** berinjela `#1F1727`, papel `#FBF7FC`, lilás-névoa `#EFE3F6`, lilás da faixada `#C48ED8`, verde-água do logotipo `#2E9C8F` / `#17766B`.
- **Estrutura:** cabeçalho em pílula flutuante, seções como blocos arredondados, coluna de avaliações fixa ao rolar no desktop, chamada final para agendar.
- **Motivo "pétala":** cantos opostos arredondados nas fotos, vindos do logotipo. Único movimento: a pétala da foto principal se abre ao carregar (respeita `prefers-reduced-motion`).
- **Sem JavaScript:** menu mobile e acordeão de serviços são só CSS.
