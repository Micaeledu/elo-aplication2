---
name: Elo Apple Repair
description: Assistência técnica de celular com busca e entrega, iPhone e Android, em Salvador (BA)
colors:
  sinal-lima: "#C7F53E"
  preto-absoluto: "#000000"
  painel-texto: "#F4F6F5"
  painel-texto-suave: "#8E9694"
  painel-linha: "rgba(255,255,255,.16)"
  papel: "#F1F3F2"
  papel-cartao: "#FFFFFF"
  texto-principal: "#080A0A"
  texto-suave: "#525A5B"
  linha-sutil: "rgba(10,12,12,.14)"
typography:
  display:
    fontFamily: "Bricolage Grotesque, Helvetica Neue, Helvetica, Arial, sans-serif"
    fontSize: "clamp(2.5rem, 5.4vw, 4.25rem)"
    fontWeight: 800
    lineHeight: 0.98
    letterSpacing: "-0.025em"
  body:
    fontFamily: "Instrument Sans, Helvetica Neue, Helvetica, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "normal"
rounded:
  pill: "999px"
  panel: "22px"
  card: "16px"
spacing:
  sm: "12px"
  md: "26px"
  lg: "52px"
  xl: "74px"
components:
  button-primary:
    backgroundColor: "{colors.sinal-lima}"
    textColor: "#000000"
    rounded: "{rounded.pill}"
    padding: "13px 20px"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.painel-texto}"
    rounded: "{rounded.pill}"
    padding: "13px 20px"
  card-quote:
    backgroundColor: "{colors.papel-cartao}"
    textColor: "{colors.texto-principal}"
    rounded: "{rounded.card}"
    padding: "28px"
---

# Design System: Elo Apple Repair

## Overview

**Creative North Star: "Sinal Verde"**

O site inteiro gira em torno de um único sinal: um verde-lima quase fluorescente pontuando um fundo preto absoluto, como a luz de "aprovado" numa bancada de conserto à noite. O resto da página é deliberadamente neutro — papel claro, texto escuro, linhas finas — para que esse verde nunca precise competir por atenção. Isso conversa direto com o posicionamento do negócio (orçamento fechado antes de qualquer reparo): o verde só aparece onde há uma decisão ou confirmação a ser tomada — o CTA de WhatsApp, a nota 5,0, o selo do passo final.

A tipografia reforça essa dualidade: uma display grotesca (Bricolage Grotesque), pesada e comprimida, para tudo que precisa "gritar" com autoridade (títulos, números, citações), e uma sans neutra (Instrument Sans) para tudo que precisa apenas ser lido sem esforço.

**Key Characteristics:**
- Um único acento de cor (verde-lima), usado com raridade extrema.
- Alternância entre painéis quase pretos (hero, CTA final) e seções em papel claro — nunca um gradiente entre os dois, sempre um corte limpo.
- Quase sem sombra; a separação vem de linhas finas e do contraste de painel, não de elevação.
- Cantos: pílula total nos botões, grande raio suave (22px) nos painéis inteiros, raio médio (16px) só nos cards de depoimento.

## Colors

A paleta é monocromática com um único acento funcional; tudo que não é o verde-lima é preto, branco ou cinza.

### Primary
- **Verde Sinal** (`#C7F53E`): o único acento do sistema. Aparece no botão de CTA, no número da nota (5,0), no glow radial do hero/CTA final e no selo do último passo do "como funciona". Nunca usado em texto de corpo ou como fundo de bloco.

### Neutral
- **Preto Absoluto** (`#000000`): fundo do hero e da seção de CTA final. Fixo — não muda com o tema claro/escuro do sistema operacional.
- **Painel Texto** (`#F4F6F5`): texto principal sobre os painéis pretos.
- **Painel Texto Suave** (`#8E9694`): texto secundário sobre os painéis pretos (legendas, sub-linhas do "facts").
- **Painel Linha** (`rgba(255,255,255,.16)`): divisórias dentro dos painéis pretos.
- **Papel** (`#F1F3F2` claro / `#0E1110` escuro): fundo das seções de conteúdo fora do hero; único token que responde ao tema claro/escuro do visitante.
- **Papel Cartão** (`#FFFFFF` claro / `#161A19` escuro): fundo dos cards de depoimento, um tom acima do papel.
- **Texto Principal** (`#080A0A` claro / `#EEF1F0` escuro): texto de corpo nas seções em papel.
- **Texto Suave** (`#525A5B` claro / `#9AA2A2` escuro): texto secundário nas seções em papel.
- **Linha Sutil** (`rgba(10,12,12,.14)` claro / `rgba(255,255,255,.16)` escuro): divisórias nas seções em papel.

### Named Rules
**The One Signal Rule.** O verde-lima nunca aparece em mais de um elemento por tela ao mesmo tempo (excluindo o glow radial de fundo). É um sinal, não uma cor de marca genérica — se ele estiver em toda parte, para de significar "aprovado".

**The Panel-or-Paper Rule.** Uma seção é ou um painel preto (hero, CTA final) ou uma seção em papel (tudo mais). Não existe meio-termo cinza entre os dois.

## Typography

**Display Font:** Bricolage Grotesque (com Helvetica Neue, Helvetica, Arial como fallback)
**Body Font:** Instrument Sans (mesmo fallback)

**Character:** A display é pesada, comprimida e de traços geométricos — carrega autoridade e urgência controlada. A body é discreta e altamente legível, feita para desaparecer atrás do conteúdo.

### Hierarchy
- **Display** (800, `clamp(40px,5.4vw,68px)`, line-height 0.98, letter-spacing -0.025em): título do hero ("Seu celular volta funcionando.").
- **Headline** (800, `clamp(30px,3.6vw,44px)`): títulos de seção (`.sec-head h2`) e do CTA final (`clamp(32px,4.4vw,54px)`).
- **Title** (600, 22px): títulos dos passos do "como funciona" (`.step h3`).
- **Body** (400, 17–18px, line-height 1.55): parágrafos de corpo; hero-lead e `.final p` usam 18px com largura máxima de ~44–46ch.
- **Label** (600, 13.5–15.5px): textos auxiliares (tags de serviço, legendas de card, telefone no header).

A display também aparece fora de títulos: no número da nota (`.rating-num`, 38px/800) e no texto dos depoimentos (`.quote p`, 20px, mas peso 400 — a única vez que a display é usada em peso leve, para um tom de citação editorial).

### Named Rules
**The Heading-Only Display Rule.** A fonte display nunca carrega texto de corpo longo; ela é reservada para títulos, números de destaque e citações curtas.

## Layout

Container com padding lateral de 74px no desktop, caindo para 40px (~960px) e 26px (~640px). Seções internas usam grids explícitos, sem sistema de coluna genérico:
- Hero: duas colunas (1.05fr / .95fr) que colapsam para uma coluna abaixo de 960px.
- Facts (3 itens): grid de 3 colunas com divisórias verticais, vira 1 coluna com divisórias horizontais no mobile.
- Como funciona: 4 passos em grid, com divisórias verticais que viram 2×2 no mobile.
- Serviços: 1fr + coluna fixa de 320px para o diagrama (diagrama é escondido abaixo de 960px).
- Depoimentos: grid de 3 colunas, 1 coluna no mobile.

Título de seção (`.sec-head`) é sempre limitado a 34ch de largura, forçando quebras de linha curtas e intencionais.

## Elevation & Depth

O sistema é essencialmente flat. Não há camadas de sombra nem elevação por hover em cards. A profundidade percebida vem do contraste entre painéis pretos e seções em papel, e de linhas finas (`--line` / `--panel-line`) separando blocos — não de `box-shadow`.

### Shadow Vocabulary
- **Glow do CTA** (`box-shadow:0 4px 20px rgba(199,245,62,.32), inset 0 1px 0 rgba(255,255,255,.5)`, mais forte no hover): único uso expressivo de sombra no sistema, reservado ao botão primário.
- **Sombra de cartão** (`box-shadow:0 1px 2px rgba(8,10,10,.04)`): quase imperceptível, só nos cards de depoimento, para separá-los do papel sem parecer "flutuante".

### Named Rules
**The Flat-By-Default Rule.** Nenhum elemento ganha sombra só por ser um "card"; sombra é reservada a ações (o botão) ou a uma separação muito sutil (cards de depoimento sobre papel).

## Shapes

- **Pílula** (`border-radius:999px`): todo botão clicável e o selo do último passo do "como funciona".
- **Painel grande** (`border-radius:22px`, token `--radius`): hero e seção de CTA final — os dois únicos blocos "objeto" da página.
- **Card médio** (`border-radius:16px`): cards de depoimento.
- **Sem raio**: facts, passos, lista de serviços, rodapé — essas áreas usam linhas divisórias, não contornos de card.

## Components

### Buttons
- **Shape:** pílula total (999px).
- **Primary:** fundo verde-lima, texto preto, padding `13px 20px`, peso 600. Único elemento com sombra própria (glow verde).
- **Hover / Focus:** brightness +6%, leve `translateY(-1px)`, glow mais forte; foco visível usa contorno verde-lima de 3px (`:focus-visible`).
- **Ghost:** fundo transparente, borda 1px `--panel-line`, texto `--panel-fg` — usado como ação secundária sobre os painéis pretos; hover ganha um fundo branco a 7% de opacidade, sem glow.

### Cards / Containers
- **Quote (depoimento):** fundo `papel-cartao`, raio 16px, padding 28px, sombra quase imperceptível. Texto do depoimento em display 400/20px; rodapé do card em 13.5px cinza.
- **Fact (bloco de destaque):** não é um card — é uma célula de grid com padding 27px/74px separada por linha, sobre o painel preto.

### Navigation
- **Header:** marca (logo + wordmark de duas linhas) à esquerda, telefone + botão CTA WhatsApp à direita. Sem estado de hover elaborado além do sublinhado padrão de link.
- **Mobile:** navegação de topo permanece, mas surge um dock fixo no rodapé da tela (`position:fixed;bottom:0`) com ligação e WhatsApp sempre visíveis — um componente exclusivo do mobile, sem equivalente no desktop.

## Do's and Don'ts

### Do:
- **Do** manter o verde-lima raro — no máximo um elemento de primeiro plano por tela usando `#C7F53E`.
- **Do** manter hero e CTA final como painéis pretos fixos (não seguem o tema claro/escuro do visitante); todo o resto responde ao tema.
- **Do** usar pílula (999px) em qualquer novo botão clicável, para consistência com os existentes.
- **Do** limitar títulos de seção a ~34ch de largura para manter as quebras de linha curtas do sistema.

### Don't:
- **Don't** adicionar sombra a facts, steps ou itens de lista de serviço — a separação nesse sistema vem de linha fina, não de elevação.
- **Don't** introduzir uma segunda cor de acento; o sistema foi desenhado para ter exatamente um.
- **Don't** usar a fonte display (Bricolage Grotesque) em parágrafos longos de corpo — ela é só para títulos, números de destaque e citações curtas.
- **Don't** misturar painel preto com papel dentro da mesma seção; a transição é sempre um corte limpo entre blocos.
