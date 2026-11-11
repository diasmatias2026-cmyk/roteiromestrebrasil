# 🎬 Roteiro Mestre Brasil

**Uma skill para o [Claude Code](https://claude.com/claude-code) que escreve roteiros de Shorts, Reels e TikTok prontos para animar e narrar** — explicadores e histórias, de 30 segundos a 3 minutos.

Ela nasceu de um teste prático: 9 skills de roteiro publicadas no GitHub foram usadas uma a uma no mesmo tema, avaliadas com nota, e o que cada uma fazia de melhor foi juntado aqui numa só. O resultado é um processo em 7 etapas que entrega o roteiro **com gancho forte, retenção, fatos conferidos e texto pronto para a voz de IA**.

---

## O que você recebe

Um arquivo `roteiro.md` com:

- ✅ **5 ganchos** de tipos diferentes, com as alavancas psicológicas marcadas — e o escolhido em **3 camadas**: o 1º quadro (funciona sem som), a fala e o texto na tela
- ✅ **Roteiro em tabela**: tempo · batida · fala · `[SHOT]` (o que se vê) · `[ON SCREEN]` (texto na tela)
- ✅ **Narração limpa**, pronta para colar no ElevenLabs ou em qualquer gerador de voz
- ✅ **Mapa de retenção**: onde cai cada gancho/rehook, o ponto de risco e o que cortar se o público sair ali
- ✅ **Checagem de fatos** com veredito e fonte para cada afirmação (✅ ⚠️ ❌ ❓ 🕒)
- ✅ **Revisão de editor** com tabela antes → depois → por quê, e a lista de nomes difíceis para ouvir antes de gerar a voz
- ✅ **Pacote de publicação**: título + 4 variações, descrição, hashtags e o 1º quadro (que vira a capa do Short)

## As 7 etapas

| # | Etapa | O que acontece |
|---|---|---|
| 1 | **Intake** | tema, tipo (explicador ou história), duração, público e objetivo; define o *payoff* antes de escrever |
| 2 | **Ganchos ★** | 5 opções, cada uma com 2–3 alavancas; você escolhe |
| 3 | **Estrutura** | gancho → super gancho → loop aberto → corpo + **rehook a cada 7–12 s** → payoff + CTA com callback ao gancho e final em loop |
| 4 | **Escrita** | frases curtas, números por extenso, `[SHOT]` + `[ON SCREEN]` em cada frase, troca visual a cada ~3 s |
| 5 | **Fatos ★** | cada afirmação conferida na web, com fonte; correção mínima |
| 6 | **Revisão** | repetições, ritmo, ponto de risco, duração a 2,5 palavras/s |
| 7 | **Entrega** | `roteiro.md` completo |

★ = a skill para e espera sua aprovação (diga "só faz" para pular).

Para **histórias**, ela usa um formato de capítulo marcado (`[IMAGEM]`, `[NARRAÇÃO]`, `[FALA: nome | tom]`, `[PAUSA]`, `[MÚSICA]`) e um **STYLE ANCHOR** que descreve os personagens do mesmo jeito em todas as cenas — ótimo para gerar imagens ou vídeos por IA sem o personagem mudar de cara.

---

## Instalação

### Opção 1 — como plugin (recomendado)
Dentro do Claude Code:
```
/plugin marketplace add diasmatias2026-cmyk/roteiromestrebrasil
/plugin install roteiro-mestre@roteiromestrebrasil
```
Reinicie o Claude Code. A skill aparece como `roteiro-mestre`.

### Opção 2 — cópia manual
```bash
git clone https://github.com/diasmatias2026-cmyk/roteiromestrebrasil.git
```
Copie a pasta `skills/roteiro-mestre` para `~/.claude/skills/` (no Windows: `C:\Users\SEU_USUARIO\.claude\skills\`).

### Opção 3 — Claude.ai / app do Claude
Compacte a pasta `skills/roteiro-mestre` em `.zip` e envie em **Configurações → Capacidades → Skills → Enviar skill**.

## Como usar

É só pedir naturalmente — a skill entra sozinha:

> escreve um roteiro de 60 segundos sobre por que o céu é azul

> quero um Short contando a história do Titanic em formato de suspense

> me dá 5 ganchos para um Reel sobre juros compostos

Dicas:
- Diga o **público** e o **objetivo** (seguir, salvar, comentar) para ganchos melhores.
- Se o seu projeto tiver um `CLAUDE.md` com o tom, o idioma e o CTA do canal, a skill segue.
- A checagem de fatos usa busca na web — deixe o navegador ou a busca do Claude disponível.

## Exemplo

Veja [`exemplos/ponte-juntas-de-dilatacao.md`](exemplos/ponte-juntas-de-dilatacao.md): um Short de ~72 s sobre por que pontes têm "buracos" (juntas de dilatação), com os 5 ganchos, a tabela de cenas, a narração limpa, o mapa de retenção, 7 fatos conferidos com fonte e a revisão. (Está em inglês porque o canal do teste é em inglês; a skill escreve no idioma do seu pedido.)

## Estrutura do repositório

```
.claude-plugin/          manifestos do plugin
skills/roteiro-mestre/
  SKILL.md               o processo em 7 etapas
  references/ganchos.md  banco de ganchos, rehooks, fechamentos e fórmulas de título
  references/formatos.md modelos de entrega (explicador e história)
exemplos/                roteiro de exemplo
```

## Inspiração e créditos

O processo foi escrito do zero, inspirado nas ideias que funcionaram melhor nestes projetos (testados em novembro de 2026):

| Ideia | Projeto |
|---|---|
| Alavancas psicológicas, 3 camadas do gancho, título + capa em par | [yaxeen/storytelling-skills](https://github.com/yaxeen/storytelling-skills) |
| Super gancho, loop aberto e rehooks a cada 7–12 s | [andreadorizza/content-creation](https://github.com/andreadorizza/content-creation) |
| `[SHOT]` / `[ON SCREEN]` por frase, texto no meio do quadro | [postoncehq/youtube-mcp](https://github.com/postoncehq/youtube-mcp) |
| Tabela de cenas com troca visual a cada 3 s, final em loop, metadados de Shorts | [AgriciDaniel/claude-youtube](https://github.com/AgriciDaniel/claude-youtube) |
| Checagem de fatos afirmação por afirmação | [lingegrace/claude-research-skills](https://github.com/lingegrace/claude-research-skills) |
| Revisão de editor para voz de IA, mapa de retenção com ponto de risco | [tubemakersoficial-rgb/kit-dark-code](https://github.com/tubemakersoficial-rgb/kit-dark-code) |
| Capítulo marcado e STYLE ANCHOR para histórias | [soul0710/story-narration-skills](https://github.com/soul0710/story-narration-skills) |

## Licença

[MIT](LICENSE) — use, modifique e compartilhe à vontade.
