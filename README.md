Iara Games

-> Plataforma brasileira de distribuição de games
-> Sprint 01 — UMA NOVA JORNADA



Contexto e Proposta do Projeto:

A Iara Games é uma plataforma de distribuição de jogos digitais inspirada na lenda da Iara, a sereia dos rios amazônicos do folclore brasileiro. A Iara é um símbolo de mistério, beleza e poder das águas, uma guardiã que encanta e atrai. Da mesma forma, minha plataforma busca encantar jogadores e conectá-los ao universo dos games de forma fluida, intuitiva e com identidade nacional.

Mas afinal, o que é a plataforma?

A Iara Games é um portal onde usuários podem:
- Descobrir, comprar e gerenciar jogos digitais;
- Explorar um catálogo de títulos nacionais e internacionais;
- Criar uma conta, montar uma biblioteca pessoal e interagir com a comunidade.

O foco desta Sprint 01 é estabelecer a fundação conceitual e visual do projeto: identidade visual definida, página inicial estática funcional e documentação clara.



Pesquisa de Plataformas de Referência:

Para entender o mercado e identificar boas práticas, pesquisei três plataformas consolidadas:

1. Steam (store.steampowered.com):
A maior plataforma de distribuição de jogos PC do mundo. Referência em:
- catálogo massivo com filtros avançados;
- sistema de avaliações da comunidade;
- biblioteca pessoal organizada por tags;
- interface densa, rica em informações.

O que aproveitei como referência: sistema de cards de jogos, organização por categorias e destaque de promoções.

2. Itch.io (itch.io):
Plataforma focada em jogos independentes (indie). Referência em:
- apoio visível a desenvolvedores independentes;
- design limpo, acessível e democrático;
- forte identidade de comunidade criativa.

O que usufrui como referência: destaque para devs nacionais e indie, foco em comunidade.

3. Epic Games Store (store.epicgames.com):
Plataforma da Epic Games com foco em exclusivos e jogos gratuitos periódicos. Referência em:
- hero section impactante com jogos em destaque;
- cards visuais com capa de jogo em formato retrato;
- ofertas e jogos gratuitos como estratégia de engajamento.

E para finalizar aproveitei a referência: hero section com destaque principal, formato retrato nos cards de jogo.



Design — Justificativas:

As decisões de design foram baseadas no conteúdo da apostila "Impactante e Funcional", que define design como o desenvolvimento de projetos que sejam ao mesmo tempo úteis, eficientes e esteticamente adequados à cultura do público-alvo.

Seguindo as etapas do processo criativo descritas no material: conhecimento, definição, associações, brainstorm e seleção, partimos do conhecimento sobre a lenda da Iara e o universo gamer para criar associações que resultaram na identidade visual: águas profundas + mistério + imersão digital.

Paleta de Cores:

A paleta foi construída em torno da essência da Iara: águas tropicais, mistério e natureza brasileira.

| Papel | Cor (hex) | Justificativa |

| Fundo principal | `#0b1a1f` | Profundeza das águas noturnas |
| Fundo alternado | `#0f2229` | Variação sutil para hierarquia visual |
| Card / superfície | `#112830` | Superfície elevada sobre o fundo |
| Borda | `#1e4a54` | Divisores sutis na mesma família |
| Destaque principal | `#4db8cc` | Água tropical iluminada — cor principal da marca |
| Brilho / ativo | `#7de0ef` | Chamadas à ação e elementos ativos |
| Acento místico | `#8b5e9e` | Referência ao lado misterioso e lendário da Iara |
| Texto principal | `#d8eef2` | Alto contraste sobre fundos escuros (≥ 4.5:1) |
| Texto secundário | `#8ab8c2` | Informações de apoio e metadados |

Tipografia:

Cinzel (Google Fonts) — títulos e logotipo  
Fonte serifada com traços clássicos e elegantes, inspirada em inscrições romanas. Transmite autoridade, mistério e atemporalidade, adequada para o caráter lendário da Iara;

Nunito (Google Fonts) — corpo de texto e interface  
Fonte sans-serif arredondada, moderna e altamente legível em telas. O arredondamento suave contrasta bem com a seriedade da Cinzel, criando equilíbrio entre o épico e o acolhedor;

Decisões Visuais:

1. Tema escuro (dark theme) 
Games são consumidos majoritariamente em ambientes com pouca luz. O tema escuro reduz o cansaço visual, valoriza as cores de destaque e cria a atmosfera imersiva característica do universo gamer, além de reforçar a ideia das "profundezas" associadas à Iara.

2. Cards com formato retrato para jogos  
O formato vertical (aspect-ratio 2:3) imita capas de jogos físicos e é o padrão consagrado em plataformas como Steam e Epic. Cria escaneabilidade visual rápida e funciona bem em grids responsivos.

3. Gradientes de fundo radiais (CSS puro)
Em vez de imagens de fundo, usamos gradientes radiais em CSS para criar profundidade e atmosfera. Isso garante carregamento rápido, visual consistente em qualquer resolução e fácil manutenção.



UX e Acessibilidade:

As decisões de acessibilidade e usabilidade do projeto foram baseadas nos conteúdos estudados nas apostilas "Internet para Todos" e "Impactante e Funcional".

Fundamentos: WCAG 2.1

Seguindo as Diretrizes de Acessibilidade de Conteúdo Web (WCAG 2.1) da W3C, buscamos atender os 4 princípios fundamentais ensinados no módulo de acessibilidade:

| Princípio - Como aplicamos:

| Perceptível | Alto contraste de cores, hierarquia visual clara, `aria-hidden` em elementos decorativos |
| Operável | Navegação completa por teclado, skip link, foco visível em todos os elementos interativos |
| Compreensível | Linguagem simples, ícones reconhecíveis, padronização de layout em todas as seções |
| Robusto | HTML semântico, atributos ARIA, compatível com leitores de tela como JAWS e NVDA |

Heurísticas de Nielsen Aplicadas:

Com base nas 10 heurísticas de Nielsen (1994) estudadas na apostila "Impactante e Funcional", aplicamos as seguintes no projeto:

Heurística 2 — Compatibilidade entre o mundo real e o sistema: 
Usamos ícones universalmente reconhecíveis (🎮 para jogos, 🔒 para segurança, 👥 para comunidade) para que o usuário identifique os elementos intuitivamente, sem precisar aprender uma linguagem nova.

Heurística 4 — Consistência e padronização:
Mesmas cores, fontes, espaçamentos e componentes (cards, botões, seções) em toda a página. Conforme Nielsen (1994), a padronização facilita a memorização e aprendizagem do sistema pelo usuário.

Heurística 8 — Estética e design minimalista: 
Cada seção contém apenas os elementos necessários para seu objetivo. Evitamos sobrecarregar visualmente o usuário com informações ou decorações que não agregam à navegação,  o que o material define como "ruído".

Outros Cuidados Implementados:

- Contraste de cores (WCAG AA)  
Todos os pares texto/fundo foram escolhidos para atingir no mínimo a razão de contraste 4.5:1 exigida pela WCAG 2.1. O texto principal (`#d8eef2`) sobre o fundo (`#0b1a1f`) supera 12:1. Conforme ensinado no módulo de acessibilidade, isso também beneficia usuários daltônicos que dependem de contraste para distinguir elementos.

- Skip link (pular para o conteúdo)  
O primeiro elemento do `<body>` é um link invisível que aparece ao receber foco via teclado (`Tab`), permitindo que usuários de leitores de tela pulem direto para o conteúdo principal, atendendo ao princípio Operável da WCAG 2.1.

- Foco visível para navegação por teclado  
Todos os elementos interativos possuem estilo `:focus-visible` com `outline` em cor de alto contraste, permitindo navegação sem mouse — recurso destacado no material como fundamental para usuários com mobilidade reduzida.

Semântica HTML e atributos ARIA  
- `role="navigation"` e `aria-label` na nav para leitores de tela como JAWS e NVDA (citados na apostila);
- `aria-label` descritivos em cards e links icônicos;
- `aria-hidden="true"` em elementos decorativos;
- Hierarquia correta de títulos (`h1` → `h2` → `h3`) em toda a página.

Responsividade:
A página adapta-se a diferentes tamanhos de tela via CSS Grid, garantindo acesso em dispositivos móveis sem JavaScript.

Preferência de movimento reduzido 
`@media (prefers-reduced-motion: reduce)` desativa todas as transições para usuários que configuraram o sistema para reduzir animações, beneficia pessoas com epilepsia fotossensível e distúrbios vestibulares.



Estrutura do Repositório


iara-games/
│
├── index.html        Página inicial (Home) — HTML + CSS
└── README.md         Documentação do projeto




- Como Visualizar

1. Clone o repositório:
   ```bash
   git clone https://github.com/SEU_USUARIO/iara-games.git
   ```
2. Abra o arquivo `index.html` diretamente no navegador.

Não foi exigido JavaScript.



Checklist da Sprint 01

- [x] Descrição da proposta da Iara Games
- [x] Pesquisa de 3 plataformas de referência
- [x] Paleta de cores com justificativa
- [x] Tipografia com justificativa
- [x] Pelo menos 3 decisões visuais justificadas
- [x] Cuidados de usabilidade e acessibilidade documentados
- [x] Página inicial estática em HTML + CSS
- [x] Sem JavaScript ou back-end
- [x] Links para as seções do site (âncoras)
- [x] README documentado



Feito por:

> Sprint 01 — Projeto Iara Games  
> Isabela Silva Santos - RM564589



*"Das profundezas das águas, a Iara canta. Da tela do computador, os games chamam."*
