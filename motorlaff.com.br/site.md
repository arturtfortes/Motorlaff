# Mapeamento estrutural do site

- URL analisada: https://www.motorlaff.com.br/
- Página analisada: Home - Motorlaff - Espaço Automotivo
- Data da análise: 2026-05-28
- Viewport analisado: desktop

---

## Elementos globais ou sobrepostos

### Copy

**Botão flutuante WhatsApp:**
- Texto do botão: "Olá Tudo bem?"
- Mensagem pré-preenchida: "Olá! Gostaria de um orçamento!"
- Posição: canto inferior direito

**Banner de cookies (cookie notice):**
- Texto: "Este site utiliza cookies para permitir uma melhor experiência por parte do utilizador. Ao navegar no site estará a consentir a sua utilização."
- Botão: "Ok"
- Botão de fechar: [ícone ×, sem texto]
- Posição: barra fixa no rodapé

### Layout

```ascii
+----------------------------------------------------------------+
| [Banner cookies — barra fixa no rodapé]                        |
| "Este site utiliza cookies..."            [Ok]  [×]            |
+----------------------------------------------------------------+

                                        [Botão flutuante WhatsApp]
                                          "Olá Tudo bem?" [ícone]
                                          (canto inferior direito)
```

### Observações estruturais

* Botão WhatsApp gerado pelo plugin QLWapp (Social Chat); abre link `api.whatsapp.com` com número (41) 3010-3333.
* Cookie notice gerado pelo plugin "Compliance by Hu-manity.co" v3.1.0, posicionado `bottom`, efeito `fade`.
* O HTML declara `lang="pt-PT"` (português de Portugal).

---

## Dobra 01 — Header / Navegação

### Copy

**Logo:** Motorlaff (imagem — logotipo da marca)

**Itens de menu:**
- Sobre nós
- Serviços
- diferenciais
- clientes
- [Botão CTA] Contato

### Layout

```ascii
+----------------------------------------------------------------+
| [LOGO]    Sobre nós    Serviços    diferenciais    clientes    |
|                                                    [Contato]   |
+----------------------------------------------------------------+
```

### Observações estruturais

* Header construído com Elementor (template de cabeçalho, ID 728), usando o tema Hello Elementor.
* Layout de 5 colunas iguais (col-16 cada): logo + 4 itens de navegação/CTA.
* Os itens de menu "Sobre nós", "Serviços", "diferenciais" e "clientes" são âncoras para seções da mesma página (`#sobrenos`, `#servicos`, `#diferenciais`, `#clientes`).
* O item "Contato" é um botão (widget button) que abre o WhatsApp com mensagem pré-definida.
* Os itens de menu (exceto o CTA) têm classe `elementor-hidden-mobile`, indicando que ficam ocultos em mobile.
* Header é fixo (posicionamento via Elementor header/footer template).

---

## Dobra 02 — Hero

### Copy

**Título (H1):**
Motorlaff

**Subtítulo / descrição:**
Oficina Mecânica especializada para o seu carro.

**CTA primário:**
Solicite um orçamento

**Coluna direita — label:**
Especializados em:

**Lista de especialidades:**
- Câmbio Automático e Manual
- Suspensão
- Freios
- Radiadores
- Embreagens
- Injeção Eletrônica
- Troca de Óleo e Filtros

### Layout

```ascii
+----------------------------+----------------------------+
|                            |                            |
|  [H1] Motorlaff            |  Especializados em:        |
|                            |                            |
|  Oficina Mecânica          |  › Câmbio Automático e     |
|  especializada para o      |    Manual                  |
|  seu carro.                |  › Suspensão               |
|                            |  › Freios                  |
|  [Solicite um orçamento]   |  › Radiadores              |
|                            |  ✓ Embreagens              |
|                            |  ✓ Injeção Eletrônica      |
|                            |  ✓ Troca de Óleo e Filtros |
+----------------------------+----------------------------+
```

### Observações estruturais

* Seção full-width com altura mínima, background via CSS (cor escura com imagem de fundo — classe `background_background: classic`).
* Layout em 2 colunas (col-50 / col-50).
* A coluna esquerda tem animação de entrada `fadeInUp`; a coluna direita tem animação `slideInRight` com delay de 550ms.
* Os primeiros 4 itens da lista usam ícone `fa-chevron-circle-right`; os últimos 3 usam `fa-check-circle`.
* O botão CTA abre WhatsApp com mensagem pré-definida.

---

## Dobra 03 — Serviços (linha 1)

### Copy

**Título da seção (H3):**
Nossos Serviços

**Card 1:**
- Título: Câmbio Automático
- Descrição: Somos especializados em manutenção e reparos de câmbio automático em Curitiba e Região.
- CTA: Solicite um orçamento

**Card 2:**
- Título: Injeção eletrônica
- Descrição: Diagnóstico preciso para problemas na injeção eletrônica em Curitiba e Região.
- CTA: Solicite um orçamento

**Card 3:**
- Título: Troca de Óleo
- Descrição: Troque óleo e filtros com os nossos profissionais capacitados em Curitiba e Região.
- CTA: Solicite um orçamento

### Layout

```ascii
+----------------------------------------------------------------+
|  Nossos Serviços                                               |
+--------------------+--------------------+--------------------+
|  [Imagem]          |  [Imagem]          |  [Imagem]          |
|  Câmbio Automático |  Injeção eletrônica|  Troca de Óleo     |
|  Somos             |  Diagnóstico       |  Troque óleo e     |
|  especializados... |  preciso...        |  filtros...        |
|  [Solicite orç.]   |  [Solicite orç.]   |  [Solicite orç.]   |
+--------------------+--------------------+--------------------+
```

### Observações estruturais

* O âncora `#servicos` está posicionado no topo desta seção.
* Seção full-width, 3 cards em 3 colunas (col-33 cada), layout image-box com imagem no topo.
* Cada card possui imagem, título H3, parágrafo descritivo e botão CTA linkando para WhatsApp.
* Imagens: fotografia real (câmbio), imagem gerada por IA (injeção), fotografia real (troca de óleo).

---

## Dobra 04 — Serviços (linha 2)

### Copy

**Card 4:**
- Título: Suspensão
- Descrição: Reparos e manutenção preventiva para a suspensão do seu veículo em Curitiba e Região.
- CTA: Solicite um orçamento

**Card 5:**
- Título: radiadores
- Descrição: Problemas com os radiadores? Nos encontraremos uma solução para o seu veículo em Curitiba e Região.
- CTA: Solicite um orçamento

**Card 6:**
- Título: freios
- Descrição: Mantenha o funcionamento dos freios em bom estado, solicite uma revisão e reparos em Curitiba e Região.
- CTA: Solicite um orçamento

### Layout

```ascii
+--------------------+--------------------+--------------------+
|  [Imagem]          |  [Imagem]          |  [Imagem]          |
|  Suspensão         |  radiadores        |  freios            |
|  Reparos e         |  Problemas com     |  Mantenha o        |
|  manutenção        |  os radiadores?... |  funcionamento...  |
|  preventiva...     |                    |                    |
|  [Solicite orç.]   |  [Solicite orç.]   |  [Solicite orç.]   |
+--------------------+--------------------+--------------------+
```

### Observações estruturais

* Seção separada (segunda linha da grade de serviços), mesma estrutura: 3 colunas col-33, image-box.
* Os títulos "radiadores" e "freios" estão em letras minúsculas no HTML original.
* Todos os CTAs linkam para WhatsApp.

---

## Dobra 05 — Sobre nós

### Copy

**Título (H2):**
+ de 20 anos de experiência!

**Parágrafo:**
Um espaço automotivo completo para você. Não é apenas um "cuidar do carro", é zelar pelo seu patrimônio da melhor maneira possível. Contamos com uma completa linha de serviços à sua disposição. Geometria, balanceamento, freios, embreagem, suspensão, troca de óleo, além de um lava-car completo, que cuida desde a lavagem até o polimento. Venha conhecer nossa empresa ou solicite um orçamento!

**CTA:**
Solicite um orçamento

### Layout

```ascii
+----------------------------+----------------------------+
|                            |                            |
|  + de 20 anos de           |  [Imagem / background      |
|  experiência!              |   de fundo — espaço        |
|                            |   visual decorativo]       |
|  Um espaço automotivo      |                            |
|  completo para você...     |                            |
|                            |                            |
|  [Solicite um orçamento]   |                            |
|                            |                            |
+----------------------------+----------------------------+
```

### Observações estruturais

* O âncora `#sobrenos` está posicionado acima desta seção (seção âncora separada vazia, ID `6c47538`).
* Layout 2 colunas (col-50 / col-50). A coluna direita contém apenas um spacer — sem texto ou imagem visível; o visual provém do background da coluna.
* A coluna esquerda tem animação `fadeInRight`.
* A seção utiliza `background_background: classic` com imagem de background aplicada na coluna direita.

---

## Dobra 06 — Banner / Imagem full-width

### Copy

[Nenhum texto visível — seção de imagem de fundo pura]

### Layout

```ascii
+----------------------------------------------------------------+
|                                                                |
|  [Imagem de fundo full-width — foto da oficina Motorlaff]      |
|                                                                |
+----------------------------------------------------------------+
```

### Observações estruturais

* Seção full-width com altura mínima, sem widgets de conteúdo visível.
* Background via slideshow Elementor com uma imagem: foto da oficina mecânica (`Oficina-mecanica-matorlaff-e1770817830872.jpeg`).
* Funciona como separador visual / break de conteúdo.

---

## Dobra 07 — Depoimentos (título)

### Copy

**Título da seção (H3):**
Depoimentos reais de nossos clientes!

### Layout

```ascii
+----------------------------------------------------------------+
|  Depoimentos reais de nossos clientes!                         |
+----------------------------------------------------------------+
```

### Observações estruturais

* O âncora `#clientes` está posicionado nesta seção.
* Seção de cabeçalho separada apenas com o título, sem depoimentos — os cards de depoimentos estão na seção seguinte.

---

## Dobra 08 — Depoimentos (cards)

### Copy

**Depoimento 1:**
- Avaliação: ★★★★★ (5 de 5)
- Texto: "Os atendentes são muito queridos, o proprietário é super atencioso, fiz uma pequena revisão no meu veículo e ele me explicou tudo certinho. Voltarei e indicarei para todos."
- Nome: Isabelle Dubik

**Depoimento 2:**
- Avaliação: ★★★★★ (5 de 5)
- Texto: "Ótima oficina com estruturas de alta qualidade e bons profissionais. Recomendo ao pessoal fazer a revisão do seu carro."
- Nome: Jefferson Sagath

**Depoimento 3:**
- Avaliação: ★★★★★ (5 de 5)
- Texto: "Excelente atendimento e serviço. Valor justo e muita transparência do que foi feito e como foi feito."
- Nome: Alan Falkoski

**Depoimento 4:**
- Avaliação: ★★★★★ (5 de 5)
- Texto: "Já foram vários serviços realizados lá e até hoje sem nenhuma reclamação. Sempre atendido com muita transparência e atenção. Preço justo e bom resultado."
- Nome: Silvio C. Neto

### Layout

```ascii
+---------------+---------------+---------------+---------------+
|  ★★★★★        |  ★★★★★        |  ★★★★★        |  ★★★★★        |
|               |               |               |               |
|  "Os          |  "Ótima       |  "Excelente   |  "Já foram    |
|  atendentes   |  oficina com  |  atendimento  |  vários       |
|  são muito    |  estruturas   |  e serviço... |  serviços...  |
|  queridos..." |  de alta..."  |               |               |
|               |               |               |               |
|  Isabelle     |  Jefferson    |  Alan         |  Silvio C.    |
|  Dubik        |  Sagath       |  Falkoski     |  Neto         |
+---------------+---------------+---------------+---------------+
```

### Observações estruturais

* 4 colunas (col-25 cada), cada uma contendo widget de avaliação (rating 5/5) + widget testimonial.
* Todos os depoimentos têm 5 estrelas.
* Os testimonials não possuem foto/avatar do autor.
* A seção seguinte (ID `28fe9e8`) é uma seção vazia (spacer).

---

## Dobra 09 — Nossos Diferenciais

### Copy

**Título da seção (H3):**
Nossos diferenciais

**Diferencial 1:**
- Ícone: dinheiro (`fa-money-bill`)
- Título: Preços Justos
- Descrição: Oferecemos serviços de qualidade com valores acessíveis e orçamento claro, sem cobranças inesperadas.

**Diferencial 2:**
- Ícone: bateria de carro (`fa-car-battery`)
- Título: Diagnóstico Rápido e Preciso
- Descrição: Equipamentos modernos permitem identificar falhas com mais rapidez e eficiência.

**Diferencial 3:**
- Ícone: estrela (`fa-star`)
- Título: Trabalho de qualidade
- Descrição: Realizamos serviços com excelência, atenção aos detalhes e mão de obra especializada.

**Diferencial 4:**
- Ícone: ampulheta (`fa-hourglass-end`)
- Título: Comodidade e Praticidade
- Descrição: Economia de tempo e menos preocupação com problemas mecânicos inesperados.

**Diferencial 5:**
- Ícone: engrenagem com pessoas (`fa-users-cog`)
- Título: Profissionais Especializados
- Descrição: Mecânicos especializados e treinados que possuem experiancia de anos.

**Diferencial 6:**
- Ícone: aperto de mão (`fa-handshake`)
- Título: Garantia de Serviço
- Descrição: Oferecemos garantia nos serviços realizados, trazendo mais tranquilidade ao cliente.

### Layout

```ascii
+----------------------------------------------------------------+
|  Nossos diferenciais                                           |
+------------------------+------------------------+-------------+
|  [ícone]               |  [ícone]               |  [ícone]    |
|  Preços Justos         |  Trabalho de qualidade |  Profission.|
|  Oferecemos serviços   |  Realizamos serviços   |  Especiali. |
|  de qualidade...       |  com excelência...     |  Mecânicos..|
|                        |                        |             |
|  [ícone]               |  [ícone]               |  [ícone]    |
|  Diagnóstico Rápido    |  Comodidade e          |  Garantia   |
|  e Preciso             |  Praticidade           |  de Serviço |
|  Equipamentos          |  Economia de tempo...  |  Oferecemos |
|  modernos...           |                        |  garantia.. |
+------------------------+------------------------+-------------+
```

### Observações estruturais

* O âncora `#diferenciais` está posicionado no topo desta seção.
* Layout: título + 3 colunas (col-33), cada coluna com 2 icon-boxes empilhados verticalmente (totalizando 6 diferenciais).
* Cada icon-box: ícone FontAwesome acima, título em `<p>` (não heading), parágrafo descritivo.
* O texto "experiancia" no diferencial 5 é um erro ortográfico presente no original.

---

## Footer — Localização e Informações

### Copy

**Coluna esquerda — título (H2):**
Nossa
localização

**Coluna direita:**
[Mapa Google Maps — embed]
- Endereço no iframe: Rua Almirante tamandaré 1275 – Juvevê – Curitiba – PR, 80040-110

---

### Copy — Barra de informações

**Coluna 1 — Contatos:**
- Título (H4): Contatos
- Telefone: (41) 3010-3333
- Email: contato@motorlaff.com.br

**Coluna 2 — Redes Sociais:**
- Título (H4): Redes Sociais
- Ícone Instagram (link para perfil do Instagram)
- Ícone WhatsApp (link para WhatsApp com mensagem)

**Coluna 3 — Endereço:**
- Título (H4): Endereço:
- Rua Almirante Tamandaré 1275,
- Juvevê - Curitiba/PR, 80040-110

**Coluna 4 — Horários:**
- Título (H4): Horarios:
- Seg - Sex: 8:00h as 18:00h
  Sab - Dom: Fechado

---

### Copy — Barra de copyright

- Motorlaff © 2026Todos os direitos Reservados
- Powered by AGÊNCIA BW

### Layout

```ascii
+----------------------------+------------------------------+
|                            |                              |
|  Nossa                     |  [Google Maps embed]         |
|  localização               |  (mapa interativo)           |
|                            |                              |
+----------------------------+------------------------------+

+---------------+---------------+---------------+------------+
|  Contatos     |  Redes Sociais|  Endereço:    |  Horarios: |
|               |               |               |            |
|  Telefone:    |  [Instagram]  |  Rua Almirante|  Seg - Sex:|
|  (41)3010-3333|  [WhatsApp]   |  Tamandaré    |  8:00h as  |
|  Email:       |               |  1275,        |  18:00h    |
|  contato@     |               |  Juvevê -     |  Sab - Dom:|
|  motorlaff    |               |  Curitiba/PR  |  Fechado   |
|  .com.br      |               |  80040-110    |            |
+---------------+---------------+---------------+------------+

+----------------------------------------------------------------+
|  Motorlaff © 2026Todos os direitos Reservados                  |
|                  Powered by AGÊNCIA BW                         |
+----------------------------------------------------------------+
```

### Observações estruturais

* Footer dividido em 3 seções HTML distintas: (1) localização full-width com mapa, (2) barra de informações em 4 colunas, (3) barra de copyright.
* A seção de localização tem animação `fadeInLeft` no título.
* O título "Nossa localização" usa quebra de linha forçada (`<br/>`) entre "Nossa" e "localização".
* O texto de copyright tem erro de formatação: "© 2026Todos" (sem espaço) — presente no original.
* O título "Horarios:" não tem acento — presente no original.
* Os itens de endereço são links clicáveis (Google Maps).
* As redes sociais exibem apenas Instagram e WhatsApp.
* Footer construído com Elementor (template de rodapé, ID 723).

---

## Variações relevantes em mobile

* Os itens de menu "Sobre nós", "Serviços", "diferenciais" e "clientes" possuem classe `elementor-hidden-mobile` — ficam ocultos no mobile; apenas o logotipo e o botão "Contato" (WhatsApp) permanecem visíveis no header mobile.
* Os botões de ação (`[Solicite um orçamento]`) têm classe `elementor-mobile-align-center`, indicando centralização em telas menores.
* Os ícones sociais no footer possuem `e-grid-align-mobile-center`, centralizando a grade em mobile.
* Não foi possível confirmar demais ajustes de layout responsivo sem renderização em viewport mobile.

---

## Inventário resumido de componentes identificados

* Header / navegação: sim
* Hero: sim
* Botões/CTAs: múltiplos (aprox. 9 ocorrências do botão "Solicite um orçamento" + 1 "Contato" no header + 1 flutuante WhatsApp)
* Cards: image-box (6 cards de serviços), icon-box (6 cards de diferenciais), testimonial (4 depoimentos)
* Formulários: não
* Depoimentos: sim (4 depoimentos com avaliação 5 estrelas)
* FAQ: não
* Footer: sim (3 subseções: mapa + info + copyright)
* Mapa: sim (Google Maps embed)
* Banner de cookies: sim
* Botão flutuante WhatsApp: sim
* Seção de imagem full-width (banner visual): sim
* Âncoras de navegação interna: 4 (`#servicos`, `#sobrenos`, `#diferenciais`, `#clientes`)
