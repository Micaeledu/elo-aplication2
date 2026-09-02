# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Moradores de Boca do Rio e bairros vizinhos (Salvador - BA) com um iPhone ou Android quebrado, molhado, sem carregar, travando ou com peça com defeito (tela, bateria, conector, câmera, botão, som).

*Inferido a partir do site (não confirmado em entrevista):* a base provável combina dois perfis — quem quer resolver sem se deslocar (usa busca e entrega) e quem está com o único celular quebrado e tem urgência alta (quer resposta e conserto rápidos). Revisitar quando houver confirmação direta do dono do negócio.

## Product Purpose

Assistência técnica de celular (iPhone e Android, todas as marcas) que busca o aparelho na casa do cliente, conserta e devolve funcionando — para quem não quer ou não pode se deslocar até uma loja.

## Positioning

Orçamento fechado antes de mexer no aparelho: o cliente manda o problema, a loja abre, testa e só conserta depois de aprovação explícita do valor. Nada é feito sem esse aceite prévio — é o diferencial que o cliente confirmou como o mais defensável frente à concorrência.

## Operating Context

- Endereço físico: R. Des. Lineu Lapa Barreto, 28, Boca do Rio, Salvador — BA.
- Atendimento também remoto via busca e entrega no endereço do cliente.
- Contato principal: WhatsApp ((71) 99392-9092), com ligação como alternativa.
- Horário: todos os dias úteis, até as 19h.
- Fluxo de atendimento em 4 passos: cliente manda mensagem (com foto, se der) → loja busca o aparelho → orçamento é passado e só é executado após aprovação → aparelho é devolvido testado e limpo no mesmo endereço.

## Capabilities and Constraints

- Conserta iPhone e Android, todas as marcas.
- Serviços cobertos: troca de tela (original ou alternativa, preço de cada uma informado antes), troca de bateria, recuperação de aparelho molhado/danos de placa, troca de conector de carga, câmera/botão/som, e problemas de software (travamentos, reinícios, tela azul) com tentativa de preservar os dados do cliente.
- Site é uma página estática (HTML/CSS, sem framework); stack já definida pelo código existente.
- Sem detalhes adicionais de garantia, política de peças ou limites de área de entrega além do que já está publicado no site — não presumir prazos, cobertura ou termos que não estejam no `index.html` atual.

## Brand Commitments

- Nome da marca: "Elo Apple Repair" (usado no título da página, header, footer e no registro do Google Maps do negócio) — mesmo consertando Android, o nome comercial não deve ser alterado sem pedido explícito do dono.
- Tom de voz: direto, coloquial, em português do Brasil ("a gente busca", "devolve na sua mão"), sem jargão técnico.
- Paleta/identidade visual atual: fundo escuro (quase preto) com verde-limão de destaque (`--lime:#C7F53E`), tipografia Bricolage Grotesque (display) + Instrument Sans (corpo).

## Evidence on Hand

- Nota 5,0 no Google com 15 avaliações, nenhuma abaixo de 5 (dado exibido no hero) — tratar como dado real do negócio, mas sujeito a mudar; não deixar hardcoded como verdade permanente em trabalhos futuros sem reconfirmar.
- Três depoimentos de clientes citados como avaliações do Google (atendimento rápido, busca e devolução de iPhone quebrado, troca de tela satisfatória) — presumir que são reais/parafraseados de avaliações existentes, não inventar novos depoimentos.
- Imagem de produto `assets/phone-hero.png` (iPhone apoiado em pedras vulcânicas, fundo azul-claro) usada no hero como substituição do antigo modelo 3D (`assets/phone.glb`, ainda no repo mas não referenciado no HTML).

## Product Principles

1. Nunca pedir para o cliente sair de casa quando puder evitar — busca e entrega é o caminho padrão, não uma exceção.
2. Preço nunca é surpresa: orçamento sempre vem antes de qualquer reparo, e o cliente aprova antes de qualquer coisa ser feita.
3. A loja atende qualquer marca (iPhone e Android) mesmo com um nome de marca "Apple Repair" — a comunicação deve deixar isso explícito sempre que citar o nome sozinho puder sugerir foco exclusivo em Apple.
4. Prova social é o que sustenta a confiança (nota 5,0, depoimentos reais) — não diluir isso com estatísticas inventadas.
