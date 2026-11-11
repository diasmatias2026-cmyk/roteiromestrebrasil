---
name: roteiro-mestre
description: Escreve roteiros de Shorts, Reels e TikTok (30 s a 3 min) prontos para animar e narrar — explicadores e histórias. Gancho com 3 camadas, estrutura de retenção com rehooks, cada frase com [SHOT] e [ON SCREEN], fatos conferidos com fonte, revisão para voz de IA, título, descrição e hashtags. Use quando o usuário pedir roteiro, script, gancho, "escreve o vídeo sobre…", ideia de Short/Reel/TikTok, ou trouxer um tema/fato para virar vídeo curto.
---

# Roteiro Mestre

Ordem fixa: **Intake → Ganchos → Estrutura → Escrita → Fatos → Revisão → Entrega**. Pare nos 2 portões (★) e espere a resposta, a menos que o usuário tenha dito "só faz".

## Padrões (valem se o usuário não disser outra coisa)
- **Idioma:** o do pedido (português do Brasil por padrão). Formato 9:16.
- **Ritmo de fala:** **2,5 palavras por segundo** (~150 por minuto). 60 s ≈ 150 palavras · 75 s ≈ 190. Nunca use 250–300 por minuto: gera roteiro com o dobro do tamanho.
- **Duração:** o conteúdo manda (30 s a 3 min). Padrão 60–75 s. Evite a faixa de 30–45 s sem motivo (pico de desempenho costuma ficar perto de 15 s ou de 60 s).
- **CTA:** o que o usuário usar no canal; sem isso, pergunte uma vez.
- Se o projeto tiver um `CLAUDE.md` ou ficha do canal (público, tom, CTA, idioma), leia e siga.

## 1. Intake (uma mensagem, no máximo 2 perguntas)
- Tema, tipo (**explicador** ou **história**), duração, público exato (quem você quer que siga, não "todo mundo"), objetivo (seguir, salvar, comentar, compartilhar).
- Antes de escrever, responda: **qual é o payoff?** — a última coisa que a pessoa leva, em uma frase. Sem payoff claro, o vídeo não está pronto.
- Se faltar informação e o usuário não puder responder, declare as premissas no topo e siga.

## 2. Ganchos ★
Leia `references/ganchos.md`. Escreva **5 ganchos** de tipos diferentes, cada um empilhando 2–3 alavancas (marque quais):
curiosidade aberta · espelho emocional · conflito (meta + obstáculo) · identificação (com palavra que qualifica o público) · padrão + surpresa · três atos.
- Funciona em menos de 2 s, uma ideia só, com objeto concreto, número ou nome em vez de categoria.
- Descarte o que seria desonesto (ex.: "acabou de sair" para algo antigo) e diga por quê.
- Proibido: saudação, nome do canal, "neste vídeo", "para de rolar", rodeios.
- Para o escolhido, entregue as **3 camadas**: **1º quadro** (funciona sem som: ação no meio, objeto estranho, antes/depois, ponto de vista do problema) · **fala** · **texto na tela** (a outra metade da lacuna — nunca repete a fala).
- Recomende 1 com o motivo e **espere a escolha**. O usuário pode misturar ou reescrever.

## 3. Estrutura
**Explicador (padrão):**
| Batida | Tempo | Função |
|---|---|---|
| Gancho | 0–2 s | o escolhido |
| Super gancho | 2–8 s | uma premissa que a pessoa já aceita OU autoridade checável (número com data, origem nomeada, prova na tela). Nunca "especialistas dizem". |
| Loop aberto | até 10 s | UMA promessa específica que só o fim paga — algo que a pessoa ganha. "Fica até o fim" não é loop. |
| Corpo → rehook × N | 10 s até o fim − 6 s | corpo = uma ideia com valor real. Rehook a cada **7–12 s** = uma frase com **informação nova** que abre um mini-loop que o corpo seguinte fecha. Proibidos rehooks vazios ("mas espera", "e não é só isso"). Por volta de 60–70% do vídeo, um rehook abre um loop novo. |
| Payoff + CTA | últimos 5–8 s | paga o loop com palavras parecidas com a promessa, faz **callback** à frase do gancho e fecha com 1 CTA. Termina quente: nada de resumo ou moral depois. |

**História:** setup (mundo normal) → problema (meta + obstáculo, sobe em 3 degraus) → virada (quebra a expectativa) → resolução (o fato ou a lição) → callback + CTA. Gancho começando no meio da ação. Cada personagem tem: quer · precisa · medo · limite · voz.

**Final em loop:** a última imagem e/ou palavra emenda no 1º quadro, para o replay.

## 4. Escrita
- Texto para ser ouvido: frases de até 25 palavras, números e siglas **por extenso** (a voz de IA lê errado), sem marcação de cena dentro da fala.
- Cada frase ganha `[SHOT: …]` (o que se vê) e `[ON SCREEN: …]` (texto curto, no meio do quadro — topo e base ficam embaixo da interface do app). Troca visual a cada ~3 s.
- Não narre o que a imagem já mostra. Números longos, comandos e nomes técnicos vão na tela, não na voz.
- História: use o capítulo marcado de `references/formatos.md` (IMAGEM / NARRAÇÃO / FALA / PAUSA / MÚSICA) e o STYLE ANCHOR.

## 5. Fatos ★ (obrigatório antes de gerar a voz)
- Extraia cada afirmação checável (número, data, nome, "o maior", causa → efeito) com um ID.
- Confira na web (navegador ou busca) e dê o veredito: ✅ apoiada · ⚠️ exagero · ❌ errada · ❓ sem fonte · 🕒 desatualizada. Anote a fonte e onde está.
- Nunca confirme pela memória nem usando outra frase do próprio roteiro. Conta feita por você = marque "cálculo" e use verbo condicional ("pode chegar a").
- Corrija com a menor mudança possível (suavizar, citar, trocar o número, cortar). Não adicione fato novo ao corrigir.

## 6. Revisão de editor
- Procure: palavras e aberturas repetidas, frases longas, o trecho com cara de aula (ponto de risco), nomes difíceis de pronunciar (liste para ouvir antes de gerar a voz).
- Conte as palavras → duração a 2,5 palavras/s; ajuste sem inventar.
- Guarde a versão anterior e mostre a tabela **antes → depois → por quê**.

## 7. Entrega
Salve em `roteiro.md` na pasta do projeto, no modelo de `references/formatos.md`:
premissas · 5 ganchos + o escolhido (3 camadas) · roteiro em tabela (tempo · batida · fala · SHOT · ON SCREEN) · **narração limpa** (só as falas, pronta para colar no gerador de voz) · mapa de retenção (onde cai cada dispositivo + ponto de risco e o que cortar) · fatos com veredito e fonte · revisão · título (3–6 palavras, até ~40 caracteres, palavra-chave na frente) + 4 variações em fórmulas diferentes · descrição (1ª linha até 125 caracteres) · 3–5 hashtags · 1º quadro (no Short ele funciona como capa) · aviso: música licenciada reduz a receita do Short.
Termine dizendo o que ficou sem conferir.
