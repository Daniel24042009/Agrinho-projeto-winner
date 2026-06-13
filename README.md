# 🌾 Raízes do Amanhã — Monitoramento de Impacto Agroecológico
> **Plataforma Interativa de Sustentabilidade Rústica e Pensamento Computacional**
> *Submetido ao Concurso Agrinho 2026 — Categoria: Programação*

---

## 📝 Sobre o Projeto
O **Raízes do Amanhã** é uma aplicação web interativa baseada no conceito de SPA (*Single Page Application*), desenvolvida para conectar estudantes, técnicos e produtores da **Escola do Campo (Antônio Olinto - PR)** às diretrizes conservacionistas de manejo da terra e preservação ambiental.

A plataforma adota uma abordagem pedagógica gamificada e científica, utilizando dados e materiais de pesquisa vinculados ao **Acervo Digital da Universidade Federal do Paraná (UFPR)** para fomentar a transição agroecológica e a literacia computacional em laboratórios de informática rurais.

---

## 🛠️ Tecnologias Utilizadas
Para garantir máxima leveza, alto desempenho e compatibilidade com computadores escolares tradicionais, o ecossistema foi estruturado puramente com tecnologias nativas da Web (*Vanilla Stack*):

* **HTML5 Estrutural:** Tags semânticas para acessibilidade e hierarquia lógica de dados.
* **CSS3 Customizado:** Design responsivo adaptado à identidade visual do campo paranaense, utilizando variáveis globais (`:root`), transições suaves e grids flexíveis.
* **Vanilla JavaScript (ES6+):** Motor lógico encarregado do controle de abas de exibição exclusivas, execução do simulador de diagnóstico, manipulação de modais informativos e gerência dos algoritmos de jogos.
* **Font Awesome & Google Fonts:** Iconografia técnica dedicada e tipografia *Plus Jakarta Sans* para leitura fluida.

---

## 🕹️ Funcionalidades Principais (Arquitetura JavaScript)

### 1. Simulador de Diagnóstico de Manejo
Um motor de avaliação matemática que calcula dinamicamente o índice de sustentabilidade de uma propriedade rural com base em quatro eixos cruciais (Solo, Água, Insumos e Biodiversidade).
* **Algoritmo de Pesos:** Distribui pontuações proporcionais conforme o nível de conservação selecionado nos elementos `<select>` do HTML.
* **Feedback Visual Instantâneo:** Atualiza elementos numéricos de progresso, redimensiona barras horizontais dinamicamente e altera o estado crítico/regular/excelente através de *badges* e caixas de alerta estilizadas.

### 2. Espaço de Capacitação Científica (Modais Dinâmicos)
Central estruturada em formato de dicionário de dados de objetos literais que gerencia as 6 grandes diretrizes agroecológicas:
* Rotação de Culturas e Cobertura
* Adubação Verde e Cobertura Viva
* MIP (Manejo Integrado de Pragas)
* SAFs (Sistemas Agroflorestais)
* Recuperação e Proteção de Nascentes
* Curvas de Nível e Terraceamento

> **Comportamento Lógico:** Ao disparar o evento de clique em um card, o script realiza uma injeção de layout assíncrona baseada em *template literals* diretamente na camada de sobreposição global (*Backdrop Overlay*).

### 3. Quiz de Fixação Continuada
Banco de dados integrado com **30 questões de múltipla escolha** divididas metodologicamente por níveis de complexidade:
* **🌱 Nível Fácil:** Conceitos básicos e princípios ecológicos.
* **🌿 Nível Médio:** Dinâmicas regulatórias e práticas gerais.
* **🌳 Nível Difícil:** Engenharia de solos, bioquímica agrícola e pedologia.
* **Destaques Técnicos:** Travamento de cliques após resposta para evitar fraude, indicação visual em tempo real (Verde para acertos / Vermelho para erros) e cálculo automático de métricas parciais.

### 4. Central de Mídias com Acervo Digital da UFPR
Um visualizador integrado embutido na interface (*Viewport Frame*) que soluciona problemas de restrição e bloqueios de segurança por *iFrames* (*X-Frame-Options*).
* **Integração Científica:** Carrega o livro técnico oficial *"Conservando os Solos"* do **Acervo Digital da UFPR** usando a API estável do *Google Docs Viewer*.
* **Mídia Audiovisual:** Carrega videoaulas práticas em formato embutido sem redirecionar ou retirar o estudante da plataforma.

### 5. Jogo da Memória com Algoritmo Fisher-Yates
Módulo gamificado para fixação ativa de termos computacionais e agrícolas que implementa o algoritmo de embaralhamento reverso **Fisher-Yates**.
* **Lógica Avançada:** Garante a aleatoriedade pura na distribuição das cartas em cada inicialização, gerencia contadores síncronos de movimentos (`moves`), cronometra o tempo de resolução e faz a verificação rigorosa de paridade em matriz bi-dimensional temporária.

---

## 📁 Estrutura do Projeto
```text
├── index.html       # Estrutura semântica e esqueleto das abas de visualização
├── style.css        # Variáveis de ambiente, design responsivo e animações 3D dos cards
└── script.js        # Lógica de controle de estado, simulador, quiz e algoritmos de jogos