🌊 Iara Games — Sprint 02

Plataforma brasileira de distribuição de games  
Sprint 02 — Aprofundamento, Formulários e Evolução da Interface

Feito por: Isabela Silva Santos — RM564589

---

Sumário

1. [Evolução da Sprint 01 para a Sprint 02](#evolução-da-sprint-01-para-a-sprint-02)
2. [Persona](#persona)
3. [ESG — Valores e Responsabilidade](#esg--valores-e-responsabilidade)
4. [Estrutura e Layout](#estrutura-e-layout)
5. [Formulários](#formulários)
6. [UI — Decisões Visuais](#ui--decisões-visuais)
7. [UX — Experiência do Usuário](#ux--experiência-do-usuário)
8. [Acessibilidade](#acessibilidade)
9. [Estrutura do Repositório](#estrutura-do-repositório)
10. [Como Visualizar](#como-visualizar)
11. [Checklist da Sprint 02](#checklist-da-sprint-02)

---

Evolução da Sprint 01 para a Sprint 02

O que foi construído na Sprint 01

A Sprint 01 estabeleceu a fundação conceitual e visual da Iara Games:
- Identidade visual definida (paleta, tipografia, dark theme)
- Página inicial estática com seções: hero, jogos, categorias, destaque, sobre e rodapé
- Documentação de acessibilidade e UX
- HTML semântico com ARIA e responsividade por CSS Grid

O que evoluiu na Sprint 02

A Sprint 02 aprofundou o projeto em três frentes principais:

1. Evolução da Home (index.html)

| Elemento | Sprint 01 | Sprint 02 |
|---|---|---|
| Hero | Título + botões | Título + badge de categoria + estatísticas da plataforma |
| Diferenciais | Embutidos em "Sobre" | Faixa visual independente com ícones e copy |
| Jogo gratuito | Mencionado no banner | Seção dedicada com card completo + CTA |
| Cards de jogos | Tags simples | Tags de "Nacional" e "Grátis" sobrepostas nas capas |
| ESG | Não existia | Nova seção com E, S, G detalhados |
| CTA final | Seção de login inline | Seção dedicada com dois botões de ação |
| Links de conta | Âncoras internas | Apontam para a nova página cadastro.html |

2. Nova Página — Cadastro/Login (cadastro.html)

Página completamente nova com dois formulários navegáveis por abas:
- Formulário de **login** com validação em JavaScript
- Formulário de **cadastro** completo com 10+ campos, validação de idade, força de senha e feedback acessível

3. Refinamento visual geral
- Sombras e bordas mais elaboradas
- Cards com hover aprimorado (maior elevação e glow)
- Painel visual imersivo na página de cadastro com gradientes radiais e "partículas" CSS
- Maior consistência nos estados de foco e interação

---

Persona

🎮 Mariana — "A Descobridora"

Perfil demográfico
- Idade: 22 anos
- Localização: São Paulo, SP
- Ocupação: Estudante de Design Gráfico
- Renda: R$ 1.200/mês (bolsa + freelas)
- Dispositivos: Notebook pessoal (principal) e celular Android

Quem é Mariana?

Mariana cresceu jogando videogame com os irmãos mais velhos e hoje é uma gamer casual-intermediária. Ela consome principalmente jogos indie e RPGs, aprecia narrativas ricas e arte brasileira. Acompanha criadores de conteúdo nacionais no YouTube e TikTok e descobre muitos jogos por recomendações de comunidade.

Tem orçamento limitado para jogos, então busca promoções, jogos gratuitos e custo-benefício. Valoriza plataformas com identidade visual cuidadosa e que "pareçam sérias" — pois já se sentiu insegura comprando em sites desconhecidos.

Objetivos
- Descobrir jogos nacionais de qualidade que se encaixem no seu estilo
- Ter uma biblioteca organizada e acessível
- Aproveitar promoções e resgates gratuitos sem complicação
- Sentir que está apoiando desenvolvedores brasileiros ao comprar

Necessidades e frustrações
- 🔴 Não quer preencher formulários longos e confusos
- 🔴 Tem medo de plataformas que não parecem seguras
- 🔴 Dificuldade em descobrir jogos indie brasileiros — eles "somem" em plataformas grandes
- 🟢 Quer navegação intuitiva e visual bonito que justifique ficar na plataforma
- 🟢 Valoriza plataformas que comunicam claramente os preços e políticas

Como a Iara Games atende Mariana
- Hero imersivo e identidade visual forte → primeira impressão de plataforma séria
- Seção de jogo gratuito em destaque → facilita o resgate mensal sem caçar o benefício
- Cards com tag "Nacional" → curadoria visível de devs brasileiros
- Formulário de cadastro com validação clara e amigável → reduz atrito e ansiedade
- Seção ESG → reforça os valores da plataforma e gera identificação

---

ESG — Valores e Responsabilidade

A Iara Games incorpora os três pilares de ESG como parte da sua proposta de valor, não apenas como discurso.

E — Ambiental (Environmental)

A distribuição 100% digital elimina:
- Produção de cartuchos, discos e embalagens físicas
- Logística e transporte de produtos
- Descarte de mídia física após uso

Cada jogo comprado na Iara Games tem pegada de carbono significativamente menor do que um equivalente físico. A plataforma não possui estoque físico, reduzindo ainda mais o impacto ambiental de toda a cadeia.

S — Social (Social)

Valorização da cultura brasileira: A identidade da plataforma é inspirada na lenda da Iara e no folclore amazônico, promovendo a riqueza cultural nacional para um público gamer que frequentemente consome referências estrangeiras.

Apoio a desenvolvedores independentes: A Iara Games prioriza visibilidade para estúdios indie e desenvolvedores brasileiros, que frequentemente não têm orçamento para competir em plataformas globais. Essa curadoria gera oportunidade econômica e representatividade.

Acessibilidade como valor social: Seguir as WCAG 2.1 não é apenas requisito técnico — é garantir que pessoas com deficiência visual, motora ou cognitiva possam usufruir da plataforma em condições de igualdade.

Jogos gratuitos mensais: O modelo de resgate gratuito reduz a barreira de acesso ao entretenimento digital para usuários de menor renda, democratizando o acesso à cultura gamer.

G — Governança (Governance)

LGPD: A plataforma coleta apenas os dados necessários, informa claramente o uso (formulário de cadastro) e não compartilha informações sem consentimento explícito.

Transparência de preços: Todos os preços, descontos e percentuais de desconto são exibidos de forma clara, sem práticas enganosas (como ocultar o preço original ou inflar artificialmente o "de").

Políticas claras de uso: Links para Termos de Uso e Política de Privacidade presentes no rodapé e no formulário de cadastro.

---

Estrutura e Layout

HTML Semântico

Ambas as páginas utilizam as seguintes tags semânticas:

| Tag | Uso |
|---|---|
| `<header>` | Cabeçalho com navegação |
| `<nav>` | Barra de navegação principal |
| `<main>` | Conteúdo principal da página |
| `<section>` | Cada bloco temático (hero, jogos, categorias etc.) |
| `<article>` | Cada card de jogo individual |
| `<aside>` | Painel visual da página de cadastro |
| `<fieldset>` + `<legend>` | Agrupamento de checkboxes no formulário |
| `<footer>` | Rodapé com links |

Organização com CSS Grid

Home (index.html):
- Hero: `grid-template-columns: 1.1fr 0.9fr` — assimetria intencional que destaca o texto
- Faixa de diferenciais: `grid-template-columns: repeat(3, 1fr)` — colunas iguais
- Jogo gratuito: `grid-template-columns: 1fr 1fr` — capa + informações
- Grid de jogos: `repeat(auto-fill, minmax(195px, 1fr))` — responsivo automático
- Grid de categorias: `repeat(auto-fill, minmax(145px, 1fr))` — responsivo automático
- Grid de pilares: `repeat(auto-fill, minmax(220px, 1fr))` — responsivo automático
- ESG: `grid-template-columns: repeat(3, 1fr)` — colunas iguais
- Rodapé: `grid-template-columns: 1.5fr repeat(3, 1fr)` — marca com mais espaço

Cadastro (cadastro.html):
- Layout principal: `grid-template-columns: 1fr 1fr` — painel visual + formulário
- Campos duplos: `grid-template-columns: 1fr 1fr` — nome/sobrenome, data/gênero
- Checkboxes: `grid-template-columns: 1fr 1fr` — preferências de gênero

---

Formulários

Página: cadastro.html

A página contém dois formulários acessíveis navegáveis por abas com padrão ARIA:

Formulário de Login

Campos:
- E-mail (type="email", autocomplete="email", required)
- Senha (type="password", minlength="6", autocomplete="current-password")
- Checkbox "Lembrar de mim"
- Link "Esqueci a senha"

Validações JavaScript:
- Campo vazio
- Formato de e-mail inválido
- Senha com menos de 6 caracteres
- Feedback de erro com `role="alert"` e `aria-live="assertive"`
- Feedback de sucesso com `role="status"` e `aria-live="polite"`

Formulário de Cadastro

Campos (10 campos + 6 checkboxes):
- Nome e Sobrenome (duplo, minlength="2", autocomplete correspondente)
- Nick de jogador (pattern para letras/números/_/-, 3-20 chars, com dica explicativa)
- E-mail (type="email", required)
- Data de nascimento (type="date", max="2007-12-31" — 18+ anos)
- Gênero (select com 5 opções inclusivas)
- Senha (minlength="8", indicador de força dinâmico)
- Confirmar senha (validação de coincidência)
- Checkboxes de gêneros favoritos de jogo (optional, para personalização futura)
- Checkbox de newsletter (opt-in explícito, marcado por padrão)
- Checkbox de termos (required, com dica de erro acessível)

Validações JavaScript:
- Nome mínimo 2 caracteres
- Nick: formato válido e mínimo 3 caracteres
- E-mail com @
- Idade mínima de 18 anos (calculada pela data de nascimento)
- Senha mínimo 8 caracteres
- Senhas coincidem
- Aceite dos termos obrigatório

Cuidados de usabilidade:
- `novalidate` no form + validação JS customizada (mensagens em português)
- `aria-invalid="true"` aplicado dinamicamente nos campos com erro
- `aria-describedby` conectando campos às suas dicas
- `aria-required="true"` em todos os campos obrigatórios
- Autocomplete correto em todos os campos de dados pessoais
- Foco movido para o campo com erro após validação
- Scroll suave até a mensagem de erro
- `role="alert"` e `aria-live="assertive"` nos erros
- `role="status"` e `aria-live="polite"` nos sucessos
- `role="progressbar"` no indicador de força da senha

---

UI — Decisões Visuais

1. Faixa de Diferenciais (nova na Sprint 02)

Decisão: Adicionar uma faixa horizontal entre o hero e o conteúdo principal com os 3 principais diferenciais da plataforma (jogo grátis, devs BR, compra segura).

Justificativa (Heurística 6 de Nielsen — Reconhecimento em vez de memorização): O usuário não precisa explorar toda a página para entender o valor da plataforma. Os diferenciais visíveis logo abaixo do hero reduzem a carga cognitiva e aumentam a confiança imediata.

2. Painel Visual na Página de Cadastro

Decisão: Layout 50/50 com painel esquerdo imersivo (gradientes, benefícios, identidade da marca) e painel direito com formulário limpo.

Justificativa (Design Thinking — Empatia): Ao chegar na tela de cadastro, o usuário está em um momento de decisão. O painel visual reforça os benefícios da plataforma no momento exato da conversão, reduzindo abandono. Referência: padrão amplamente validado por plataformas como Notion, Linear e Figma.

3. Indicador de Força de Senha

Decisão: Barra de progresso colorida com rótulo textual que reage em tempo real à senha digitada.

Justificativa (Heurística 1 de Nielsen — Visibilidade do status do sistema): O usuário precisa de feedback imediato sobre a qualidade da senha. A barra visual + texto ("Muito fraca", "Boa", "Muito forte") comunica o estado de forma acessível tanto para usuários visuais quanto para leitores de tela (via `aria-live`).

4. Seção ESG com Letras em Destaque

Decisão: Cards com a letra E, S ou G em tamanho 3.5rem e cor semitransparente como elemento decorativo de fundo.

Justificativa (Hierarquia Visual — apostila "Impactante e Funcional"): A letra grande cria identidade visual para cada card, facilita a navegação visual rápida e mantém coerência com o uso da tipografia Cinzel — que tem caráter épico e atemporal, adequado para comunicar compromissos institucionais.

5. Tags "Nacional" e "Grátis" nos Cards de Jogos

Decisão: Tags sobrepostas no canto superior esquerdo das capas dos jogos, com cores distintas (verde para grátis, azul/escuro para nacional).

Justificativa (Heurística 2 de Nielsen — Compatibilidade com o mundo real): Em plataformas físicas (prateleiras de loja), produtos possuem etiquetas de destaque. A transposição desse padrão para o digital é intuitiva e facilita a filtragem visual pelo usuário sem precisar abrir cada card.

---

UX — Experiência do Usuário

Design Thinking Aplicado

Seguindo as etapas da metodologia Design Thinking estudadas na apostila "Impactante e Funcional":

Empatia: A persona Mariana foi criada com base em características reais do público gamer brasileiro jovem — estudante, orçamento limitado, valoriza identidade cultural e desconfia de plataformas desconhecidas. Essa empatia guiou as decisões de conteúdo (jogo gratuito em destaque, seção de devs BR) e de formulário (mensagens de erro amigáveis em português, validação de idade explicada).

Definição: O problema central de Mariana é: "Quero descobrir e acessar jogos nacionais de qualidade com segurança e sem burocracia."

Ideação: Exploradas soluções como: jogo gratuito mensal em destaque (modelo Epic Games), painel visual na tela de cadastro para reduzir abandono, checkboxes de preferência para personalização futura.

Prototipagem: As páginas HTML+CSS constituem o protótipo navegável de alta fidelidade entregue nesta sprint.

Teste: Embora testes com usuários reais estejam fora do escopo desta sprint, a validação contra as heurísticas de Nielsen e os princípios WCAG 2.1 serviu como método de verificação sistemática.

Fluxo do Usuário Principal

```
Home (index.html)
  └─ Hero: "Criar conta grátis" ──────────► cadastro.html (aba Cadastro)
  └─ Nav: "Entrar" ───────────────────────► cadastro.html (aba Login)
  └─ Jogo gratuito: "Resgatar agora" ────► cadastro.html (aba Cadastro)
  └─ CTA final: "Já tenho conta" ────────► cadastro.html (aba Login)
```

Heurísticas de Nielsen Aplicadas na Sprint 02

Heurística 1 — Visibilidade do status do sistema:
Indicador de força de senha em tempo real + mensagens de sucesso e erro com feedback imediato após submit.

Heurística 5 — Prevenção de erros:
`type="email"`, `type="date"`, `minlength`, `maxlength`, `pattern` no HTML + validação JavaScript antes do submit, com foco automático no campo com erro.

Heurística 7 — Flexibilidade e eficiência:
Abas Login/Cadastro permitem alternância rápida. Link "Já tem conta?" dentro do formulário de cadastro evita que o usuário precise procurar o acesso alternativo.

Heurística 9 — Ajudar usuários a reconhecer, diagnosticar e corrigir erros:
Mensagens de erro em primeira pessoa, claras e específicas: "Informe um e-mail válido", "As senhas não coincidem", "Você deve ter 18 anos ou mais" — sem jargão técnico.

---

 Acessibilidade

 WCAG 2.1 — Princípios Aplicados

Perceptível:
- Todos os campos obrigatórios marcados com `*` e `aria-label="campo obrigatório"`
- Dicas de preenchimento associadas via `aria-describedby`
- Mensagens de erro e sucesso com `role="alert"` / `role="status"` + `aria-live`
- Barra de força de senha com `role="progressbar"` e `aria-valuenow`

Operável:
- Skip link no topo de ambas as páginas
- Todos os elementos interativos acessíveis por teclado (Tab, Enter, Space)
- Foco visível com `outline` de alto contraste
- Abas do formulário com `role="tab"`, `aria-selected` e `aria-controls`

Compreensível:
- Labels explícitos para todos os campos de formulário (`for` + `id`)
- `fieldset` + `legend` para agrupar checkboxes relacionados
- Mensagens de erro em português, claras e acionáveis
- `autocomplete` correto em campos de dados pessoais

Robusto:
- HTML semântico com hierarquia correta de títulos (h1 → h2 → h3)
- `novalidate` + validação JS garante controle sobre as mensagens (sem mensagens nativas do browser em inglês)
- `aria-invalid="true"` aplicado dinamicamente

Responsividade

- Home: menu de navegação ocultado em mobile (`display: none` abaixo de 768px — melhoria futura: hamburger menu)
- Cadastro: painel visual ocultado em mobile, formulário ocupa 100% da largura
- CSS Grid com `auto-fill` e `minmax` garante adaptação automática dos cards
- `@media (prefers-reduced-motion: reduce)` desativa todas as transições

---

Estrutura do Repositório

```
iara-games/
│
├── index.html        Página inicial (Home) — Sprint 02 evoluída
├── cadastro.html     Página de Login e Cadastro (nova na Sprint 02)
└── README.md         Documentação atualizada — Sprint 02
```

---

Como Visualizar

1. GitHub:
```
https://github.com/bebel127/iaragames
```

2. Abra o arquivo `index.html` diretamente no navegador.

3. Para navegar entre as páginas, use os links da navegação:
   - "Entrar" leva para `cadastro.html`
   - "Criar conta grátis" leva para `cadastro.html`
   - Logo e "← Voltar" retornam para `index.html`


---

Checklist da Sprint 02

- [x] Persona definida com perfil, objetivos, necessidades e relação com o projeto
- [x] Relação do projeto com valores ESG (Ambiental, Social e Governança)
- [x] HTML semântico em todas as páginas
- [x] Organização de layout com CSS Grid
- [x] Evolução da Home em relação à Sprint 01
- [x] Criação de nova página (cadastro.html)
- [x] Formulário de login com validação
- [x] Formulário de cadastro com 10+ campos e validação
- [x] Sem back-end
- [x] Cuidados de usabilidade e acessibilidade nos formulários
- [x] Refinamento visual em relação à Sprint 01
- [x] Justificativa das decisões de UI e UX
- [x] README atualizado com conteúdo conceitual completo

---

> Iara Games· Sprint 02 — UMA NOVA JORNADA  
> Isabela Silva Santos — RM564589  
> Feito com 💙 no Brasil
