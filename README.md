# Treino de Cálculo Mental

Aplicação em um único arquivo HTML (Vue 3 via CDN) para treinar cálculos mentais, com geração de operações, verificação automática, cronômetros, pontuação e progressão de níveis.

## Como usar

Abra `index.html` no navegador. Configure a operação e a quantidade de dígitos (configurações avançadas ficam recolhidas). Responda às operações; acertos e erros são contabilizados.

## Implementado

- **Operações básicas:** soma, subtração, multiplicação, divisão.
- **Operações avançadas:** potência, raiz quadrada, porcentagem, frações (soma de frações com mesmo denominador).
- **Modo misto** (todas as operações).
- **Configuração de dígitos** por operando (1–4) e **quantidade de operandos** (2–4).
- **Geração inteligente:** subtração não negativa, divisão exata, porcentagem inteira.
- **Verificação automática:** ao digitar a resposta correta ou errada, a próxima operação é gerada automaticamente.
- **Cronômetro por operação** e **cronômetro de sessão**, com fim automático da sessão.
- **Pausar/retomar** sessão mantendo o tempo restante.
- **Pontuação por velocidade** (bônus pelo tempo restante).
- **Níveis de dificuldade:**
  - Modo manual (configuração livre).
  - Modo automático com progressão: sobe após 3 acertos seguidos, desce após 2 erros seguidos (6 níveis).
- **Persistência local** (estatísticas, configurações, nível, pontuação) via `localStorage`.
- **Interface organizada:** operações principais visíveis, demais em painel avançado colapsável; selects para configurações; spinners do input numérico removidos; badge compacto de nível; responsividade básica.
- **Histórico persistente de sessões** com data, pontuação, acertos/erros, aproveitamento e melhor pontuação.
- **PWA:** manifest, ícone, service worker com cache offline e botão de instalação.
- **Feedback sonoro e visual:** beep para acerto/erro e animações (pop/shake) no feedback.
- **Modos de jogo:** livre, desafio por vidas (3 vidas) e desafio por tempo.
- **Estatísticas avançadas:** tempo médio por operação, desempenho por tipo de operação.
- **Testes automatizados básicos:** `tests.html` (redireciona para `index.html?test=1`) executa autoverificações de geração/verificação.

## Pendente / Próximas evoluções

- Cronômetro com pontuação mais refinada e ranking de velocidade.
- Níveis com critérios adicionais (tempo médio, precisão) e mais faixas.
- Novos modos: potência/raiz com expoentes variáveis, porcentagens compostas, frações com denominadores diferentes, decimais.
- Histórico/ranking com mais detalhes e filtros (já há versão básica).
- Modos treino vs. desafio com mais variantes (vidas, tempo, desafios diários) — básico implementado.
- Acessibilidade (atalhos de teclado, leitura de tela, alto contraste).
- PWA com notificações (básico de instalação/offline implementado).
- Estatísticas avançadas com gráficos (básico implementado).
- Multiplayer/compartilhamento de desafios e pontuação.
- Internacionalização (outros idiomas).
- Testes automatizados mais abrangentes (básico implementado).
- Refatoração em componentes (Vite) mantendo opção de arquivo único.
- Melhorias de UX: modal de configurações, temas, atalhos, onboarding.