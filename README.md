# Prompt de imagem

Guia visual: abra o `COMO-FUNCIONA.html` desta pasta (dois cliques; funciona sem internet).

Escreve o texto (prompt) para colar numa ferramenta de gerar imagem com IA: prompt principal, o que evitar, três variações e o que ajustar se vier errado. Antes, confere na documentação atual da ferramenta o que ela aceita. Não gera a imagem.

## Como instalar

**Direto do GitHub:** no Claude Code, diga: "Instale a skill a partir de https://github.com/Empire-Business/omnx-imagem-criar-prompt". Para atualizar, diga: "Atualize a skill a partir de https://github.com/Empire-Business/omnx-imagem-criar-prompt". A IA baixa e copia os arquivos.

Se você já baixou esta pasta:

1. Abra o Claude Code (aplicativo do Claude, aba **Code**, ambiente **Local**).
2. Escreva: **"Instale a skill omnx-imagem-criar-prompt a partir desta pasta: `<caminho desta pasta>`"**.
3. A IA copia a skill para o lugar certo. Você não digita comando nenhum e vê um aviso de que terminou.
4. Abra uma conversa nova e peça, por exemplo: **"Cria um prompt para uma foto do meu produto em cima de uma mesa de madeira."**.

### Instalar à mão

- **Mac ou Linux:** rode `bash install.sh` nesta pasta (dá para rodar de qualquer lugar, com o caminho entre aspas). A skill vai para `~/.claude/skills/omnx-imagem-criar-prompt`. Se editar algo aqui, rode de novo.
- **Windows:** copie esta pasta, sem o `install.sh`, para `%USERPROFILE%\.claude\skills\omnx-imagem-criar-prompt`. Ou peça para a IA fazer isso.

## O que ela não faz

- Não gera o arquivo da imagem.
- Não imita artista, estúdio ou marca: descreve a técnica.
- Não usa rosto de pessoa real sem autorização.
- Capa no molde é da `omnx-imagem-criar-capa`; vídeo, da `omnx-video-criar-prompt`; site e identidade visual, do Morfo.

## Pedidos que funcionam

- "Cria um prompt para uma foto do meu produto em cima de uma mesa de madeira."
- "Melhora esse prompt de imagem que eu escrevi."
- "Quero uma ilustração para um post sobre organização financeira."
- "Como peço essa imagem para a minha ferramenta de IA?"

## Outro sistema operacional e outra ferramenta

As seções "Outro sistema operacional" e "Outra ferramenta (Codex e outras)" do `SKILL.md` dizem à IA o que adaptar. Feita e testada no Claude Code em macOS. **Não foi testada no Codex** nem no Windows e Linux: a IA da pessoa adapta ao instalar e conta o que funcionou.
