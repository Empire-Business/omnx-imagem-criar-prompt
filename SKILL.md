---
name: omnx-imagem-criar-prompt
description: "Escreve um prompt pronto para colar numa ferramenta de gerar imagem com IA, com o que evitar, três variações e o que ajustar se vier errado, conferindo na documentação atual da ferramenta o que ela aceita. Use quando pedirem 'cria um prompt de imagem', 'prompt para gerar essa foto', 'como peço essa imagem para a IA', 'melhora esse prompt de imagem', 'descreve essa arte para eu gerar', foto de produto, ilustração, arte para post, banner ou mockup gerado por IA. Só escreve o prompt: não gera o arquivo. Não use para capa de curso, capa de plataforma, thumbnail ou flyer no molde fixo (omnx-imagem-criar-capa), prompt de vídeo (omnx-video-criar-prompt), figura científica (lucia), site ou identidade visual (morfo), nem para instruções de agente ou chatbot (agenor)."
---

# Criar prompt de imagem

Entrega um pacote pronto para colar na ferramenta de imagem da pessoa: prompt principal, o que evitar, três variações e o que ajustar se vier errado. Não gera a imagem.

## Como conversar

Quem usa pode nunca ter gerado uma imagem. Se a pessoa chegar sem contexto, diga em duas linhas o que você faz e pergunte o que ela quer ver na imagem. Uma pergunta por vez. Palavra técnica vem com meia frase de explicação. Toda resposta termina com o próximo passo. A pessoa nunca precisa digitar comando.

## Passos

1. **Junte o pedido.** Use o que a pessoa já disse e pergunte só o que muda a imagem. Sem isto não dá para começar: **o que aparece** e **onde a imagem vai ser usada**. O resto você decide e declara no pacote: estilo, clima, luz, proporção. Pergunte também qual ferramenta ela usa. Se não souber ou não tiver uma, siga com prompt em linguagem natural e avise.
2. **Confira a ferramenta na documentação atual.** Busque a página oficial da ferramenta e veja: como ela prefere receber o prompt, em que idioma, se aceita imagem de referência, se tem campo para o que evitar, como define proporção, como lida com texto dentro da imagem, quais parâmetros existem hoje. Anote o link e a data. Só conta a documentação oficial: blog, fórum e vídeo não servem. Se o que ela diz depender da versão, pergunte a versão uma vez; sem resposta, diga no pacote para qual versão cada coisa vale. Não escreva parâmetro, versão ou modelo de memória: eles mudam. Sem acesso à documentação ou sem resposta clara, entregue em linguagem natural, sem parâmetros, e escreva "não conferi os parâmetros desta ferramenta".
3. **Monte o prompt nesta ordem:** sujeito, ação ou posição, lugar, luz, técnica ou estilo, cores, composição e câmera, clima. Parâmetros, se a documentação confirmou, vão onde ela manda. Troque tudo que é vago por algo que dá para fotografar ou desenhar. Consulte `references/vocabulario-visual.md` quando faltar palavra ou quando o pedido for de um tipo listado lá. Escreva no idioma que a documentação recomenda. Sem orientação, use inglês na descrição e mantenha no idioma da peça, entre aspas, o texto que deve aparecer na imagem.
4. **Escreva o que evitar.** Só o que tem chance real de aparecer neste pedido, não uma lista genérica. Se a ferramenta não tiver campo para isso, leve para dentro do prompt como pedido afirmativo ("fundo liso e vazio" em vez de "sem objetos no fundo").
5. **Faça três variações**, cada uma mudando um eixo só, com o prompt inteiro: A muda a composição, B muda a luz, C muda a técnica ou o estilo. Assim a pessoa compara e sabe o que mudou.
6. **Confira antes de entregar:**
   - Dá para imaginar a mesma cena lendo o prompt duas vezes? Se dois leitores imaginariam coisas diferentes, falta concreto.
   - Há pedidos que se contradizem (luz dura e sombra suave, por exemplo)?
   - Saiu nome de artista, marca ou obra? Troque (veja Regras).
   - O texto da imagem está curto, entre aspas e escrito exatamente como deve sair?
7. **Entregue no formato abaixo**, na conversa. Salve em arquivo só se a pessoa pedir, no lugar que ela indicar.

## Regras

- **Estilo sem imitação.** Nunca peça "no estilo de" um artista, ilustrador, estúdio ou marca. Se a pessoa pedir, diga em uma frase por que trocou e descreva a técnica no lugar: traço, material, paleta, composição.
- **Rosto de pessoa real** só com foto enviada pela própria pessoa ou com autorização dela, dita na conversa. Nunca figura pública, famoso, concorrente ou alguém que não sabe que está sendo usado. Sem foto, descreva um personagem fictício.
- **Nada que engane:** recibo, documento, notícia, antes e depois ou prova de resultado feitos com IA para parecer real. Recuse a parte e ofereça uma versão honesta.
- **Não invente recurso da ferramenta.** Sem confirmação na documentação, não existe.
- **Imagem de referência:** se a pessoa enviar uma, descreva o que observa nela (assunto, luz, cores, enquadramento) antes de montar o prompt.

## Formato de entrega

```
## Imagem: <nome curto>

Ferramenta: <nome e versão, ou "não informada">
Documentação: <link e data, ou "não conferi os parâmetros desta ferramenta">
Uso: <onde vai>  |  Proporção: <ex.: 4:5>

### Prompt principal
<prompt completo, em bloco de código>

### O que evitar
<bloco de código, ou "esta ferramenta não tem campo próprio: já incluí no prompt">

### Variações
A, composição: <prompt completo>
B, luz: <prompt completo>
C, técnica: <prompt completo>

### Se vier errado
<2 ou 3 ajustes específicos deste pedido: o que trocar, e em qual parte do prompt>

Próximo passo: <o que a pessoa faz agora>
```

## Exemplo de troca do vago pelo concreto

Pedido: "uma foto bonita de café para o Instagram".
Fraco: `beautiful coffee photo, high quality, aesthetic`.
Bom: `A ceramic espresso cup on a worn oak table, thin steam rising, soft side light from a window on the left, warm brown and cream tones, close-up from a low angle, empty wall behind, calm early-morning mood`.

## Outro sistema operacional

Esta skill não tem script: só conversa e escreve texto, então funciona igual em macOS, Windows e Linux. Adapte o que for preciso e conte à pessoa o que realmente testou.

- **Instalar:** no Windows, copie esta pasta, sem o `install.sh`, para `%USERPROFILE%\.claude\skills\omnx-imagem-criar-prompt`. No Mac e no Linux, rode o `install.sh`.
- **Caminhos:** `~` é a pasta do usuário; no Windows é `%USERPROFILE%`. Caminho com espaço vai entre aspas.
- **Abrir um arquivo salvo para a pessoa:** `open` (macOS), `start ""` (Windows), `xdg-open` (Linux).

## Outra ferramenta (Codex e outras)

Compatível com Claude Code, Codex e outras ferramentas de agentes, em Mac, Windows e Linux. Se a pessoa pedir para instalar
fora do Claude Code, a IA dela adapta na hora, testa no computador dela e conta o que realmente funcionou:
- **Onde pôr os arquivos:** confira na documentação atual da ferramenta. No Codex, a referência em 08/11/2026 era `~/.agents/skills/<name>`.
- **Referências:** `references/...` é relativo à pasta onde este `SKILL.md` ficou instalado.
- **Pesquisa na internet:** se a ferramenta não pesquisar, siga o passo 2 como "sem acesso à documentação".
