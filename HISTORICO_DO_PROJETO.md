# 📜 Histórico do Projeto — Portal do Engenheiro Mágico / Reino Estrutural

> Documento de referência. Atualizar conforme o projeto evolui. Ideal pra ficar na **Base de Conhecimento** do Projeto no Claude (não nas Instruções).

## Visão Geral

Plataforma didática de longo prazo (apps, sites, jogos, vídeos, animações) ensinando engenharia civil de forma lúdica, através de um "Reino Mágico" fantástico, com o objetivo de cativar jovens pra área.

**Tecnologia atual:** protótipo em arquivo HTML único, com React carregado via CDN + Babel standalone (tradução em tempo real no navegador). Sem backend, sem persistência de dados ainda.

**Arquivos:** `reino_estrutural_v1.html` até `v12.html` (cada versão = uma rodada de mudanças; ver Changelog abaixo pra saber o que mudou em cada uma).

---

## 1. Changelog (o que já foi feito)

**v1 — Base original** (arquivo enviado pelo usuário)
Mapa mental React: Esqueleto (Análise Estrutural) e Músculos (Resistência dos Materiais), os 5 Vilões (tração/compressão/flexão/torção/cisalhamento), curiosidades pré-carregadas, quiz de 1 pergunta. Bug: imagem `image_13.png` quebrada.

**v2 — Identidade visual**
Paleta (noite/pedra/dourado/verde-água/pergaminho/vermelho-selo), fontes Cinzel+Nunito, Portal Mágico em SVG (substitui a imagem quebrada), fundo noturno com estrelas.

**v3 — Topo medieval**
Céu pôr-do-sol, montanhas em SVG, castelo gótico (torres assimétricas, janelas ogivais), estandarte "O GRANDE REINO DAS ESTRUTURAS", placas "Reino do Esqueleto" / "Reino do Músculo".

**v4 — Portal aprimorado + Mago Aurelius**
Portal Central com moldura de pedra, anéis rúnicos girando, faíscas. Mascote **Mago Aurelius** criado: avatar fixo, balão de fala, 7 falas que alternam a cada clique.

**v5 — Blocos redesenhados (1ª versão)**
"Placas de pedra" (nós-pai) e "cartas de feitiço" (nós-folha), trilha rúnica, losango dourado como ícone de expandir/fechar.

**v6 — Correção de contraste**
Moldura dupla (funciona sobre qualquer cor de fundo), trilha rúnica mais grossa/brilhante.

**v7 — Fundo dinâmico**
Céu fixo (acompanha rolagem), lua, 24 estrelas piscando, 3 estrelas cadentes, névoa mágica, nuvens, dragão, poeira mágica, vinheta+grão, chão do reino.

**v8 — Correção de bug + vivacidade**
Bug corrigido: vinheta tampava estrelas/lua (movida pra dentro do `background`). Cores mais vibrantes, lua maior, névoa trocada por véus de aurora (a versão anterior "parecia holofote de festa"), dragão com voo orgânico (2 elementos aninhados).

**v9 — Escudos dos 2 reinos principais**
`analise` e `resmat` ganham escudo SVG customizado (metal + círculo técnico-mágico + emblema). Esqueleto: caveira + treliça estrutural. Músculo: bíceps + setas de compressão. Efeitos de clique: faísca (Esqueleto) e brilho (Músculo).

**v10 — Espadas nos nós-folha**
Escudos reduzidos (150×165px). Todos os nós-folha viram espadas completas (substituem o card retangular). Metal por categoria: **prata** (Esqueleto), **bronze** (Músculo), **ferro escuro + fio vermelho** (os 5 Vilões).

**v11 — Correção de bug + fundo de pedra**
Bug corrigido: fundo branco padrão do navegador na espada (CSS faltando). Fundo "pergaminho" (creme claro) redesenhado como laje de pedra escura reforçada com metal — não combinava mais com blocos metálicos. Textos ajustados pra legibilidade.

**v12 — Painel do Reino**
Border-radius uniformizado (12px). Novo painel: 2 anéis de progresso animados + card de tempo, 6 coroas de conquista (2 acesas/4 bloqueadas), galeria dos 6 reinos/módulos (4 novos escudos: Introdução/bronze-envelhecido, Sistemas Construtivos/terracota, Mecânica dos Sólidos/grafite-azul, Estruturas/índigo — bloqueados com corrente+cadeado), 2 águias heráldicas decorativas. **Dados de exemplo (fake), sem sistema real ainda.**

**Outros marcos (não-visuais):**
- Recebido e analisado documento Word "O Esqueleto Invisível do Mundo" (656 linhas, história alternativa/bem-humorada da engenharia civil, 2 partes que batem com os 6 módulos). Só leitura feita, conteúdo ainda não integrado ao código.
- Definida trilha de 6 módulos de conteúdo (ver Glossário).
- Decisão técnica: continuar em HTML por enquanto, migrar pra projeto real (React+Vite / possivelmente Phaser-Godot) só quando o conteúdo estiver validado.

---

## 2. Em Andamento

- Organização da documentação do projeto (este documento).

---

## 3. Roadmap (decidido, falta construir)

- [ ] Usuário vai apresentar as ideias pro **"end"** (sistema de progressão real, desbloqueios) — ainda não compartilhadas.
- [ ] Encaixar as curiosidades do Word no projeto (formato a definir: leitura longa / hooks curtos / linha do tempo / mistura).
- [ ] Sistema de dados real (localStorage) pra substituir os números fake do Painel do Reino.
- [ ] Decidir sobre inserção de vídeo MP4 (adiado; problema técnico real de tamanho de arquivo/link quebrado).
- [ ] Linha do tempo interativa da história da engenharia (cronologia aprovada, não implementada).
- [ ] Expandir os 4 módulos restantes como nós reais na árvore (hoje só 2 de 6 existem de verdade: Análise Estrutural e Resistência dos Materiais) — pré-requisito pros novos brasões terem conteúdo de verdade por trás.

---

## 4. Backlog (ideias, não comprometidas ainda)

- Cartas de feitiço colecionáveis
- Laboratório do Mago (sandbox de testar materiais)
- Trilha em mapa estilo RPG (ilhas conectadas por pontes)
- Diário do Engenheiro (selos de progresso) — pré-requisito pras coroas funcionarem de verdade
- Comparação "Mundo Real vs Reino Mágico"
- Modo Desafio Relâmpago (com timer)
- Quiz expandido (banco de perguntas + pontuação real)
- Sons + narração por voz (Web Speech API)
- Correntes/cadeado funcionais (depende do sistema de progressão real)
- Mais elementos heráldicos (grifos, leões, cruzes, flor-de-lis decorativos)

---

## 5. Decisões e Porquês

| Decisão | Porquê |
|---|---|
| HTML único + React via CDN (não projeto real ainda) | Prototipar rápido e barato enquanto conteúdo/ideias ainda mudam muito |
| CSS/SVG em vez de imagens externas | Já tivemos bug de imagem quebrada (`image_13.png`); SVG não depende de arquivo externo |
| Elementos heráldicos desenhados do zero | Referência enviada era de banco de imagens com marca d'água (direito autoral); SVG próprio mantém o arquivo autocontido |
| Metal diferente por categoria nas espadas | Reforça o código de cores sem pintar a lâmina inteira (mais realista) |
| Painel do Reino com dados fake por enquanto | Usuário quis visualizar o design antes de conectar dados reais |
| Fundo pergaminho claro → pedra escura | Parou de combinar quando os blocos ganharam visual metálico pensado pra fundo escuro |

---

## 6. Glossário

| Termo | Significado |
|---|---|
| **Mago Aurelius** | Mascote fixo (🧙‍♂️), canto inferior direito, fala frases aleatórias ao clicar |
| **Reino do Esqueleto** | Módulo "Análise Estrutural" (nó `analise`), cor verde-água, metal prata |
| **Reino do Músculo** | Módulo "Resistência dos Materiais" (nó `resmat`), cor dourada, metal bronze |
| **Os 5 Vilões** | Tração, Compressão, Flexão, Torção, Cisalhamento — metal ferro escuro + fio vermelho |
| **Painel do Reino** | Seção de estatísticas/dashboard visual (progresso, conquistas, galeria de módulos) |
| **Portal Central** | Elemento SVG circular com anéis girando; abre curiosidade geral ao ser clicado |
| **Os 6 Módulos** | 1. Introdução à Engenharia · 2. Sistemas Construtivos · 3. Mecânica dos Sólidos · 4. Análise Estrutural · 5. Resistência dos Materiais · 6. Estruturas |

