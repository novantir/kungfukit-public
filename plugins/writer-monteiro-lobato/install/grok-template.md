<!-- install/grok-template.md -->
# Publicar na loja do Grok Bot

Um modelo (template) do Grok Bot é um link público: quem o abre clica em "Add to Grok Bot" e recebe uma cópia do Bot. Só personas sobre obras em domínio público, com "(IA)" no nome, podem ser publicadas; personas de uso pessoal, personificações e personas sobre obras protegidas não vão para espaço compartilhado. Quem publica responde pelo modelo perante os termos de bots de terceiros da xAI.

Verificado numa conta real em 2026-11-04: o modelo leva a descrição do perfil (mostrada como "Instruções"), as memórias e o texto das habilidades, e não leva arquivos. Um Bot importado ignorou a memória "releia o SKILL.md" e respondeu sem a persona; com a regra permanente na descrição, o Bot importado se apresentou como a persona e disse a versão. O download pela regra só foi testado dentro da mesma conta, em que os Bots compartilham o computador e a pasta já existia.

## 1. Instale a persona

Crie o Bot "Monteiro Lobato (IA)" como [install/grok-bot.md](grok-bot.md) explica e confira que ele se apresenta e diz a versão.

## 2. Ponha a regra permanente na descrição

Envie ao Bot "Monteiro Lobato (IA)" (o Bot principal não edita o perfil de outro Bot):

> Substitua a sua descrição exatamente por este texto, sem mudar nada, e confirme se coube inteira ou se foi cortada:
>
> Persona de IA inspirada nas obras em domínio público de Monteiro Lobato (1882–1948), publicadas até 1930: conta e inventa histórias no estilo dele para crianças e adultos, conversa sobre o Brasil… REGRA PERMANENTE: antes de cada resposta, leia /workspace/personas/writer-monteiro-lobato/SKILL.md e siga-o; os caminhos citados nele são relativos a essa pasta. Se a pasta não existir, primeiro baixe SKILL.md, references/knowledge.md e references/evidence.md de https://raw.githubusercontent.com/novantir/kungfukit-public/main/plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/ para ela, sem alterar nada. Você é uma persona de IA inspirada nas obras de Monteiro Lobato, não Monteiro Lobato. Nunca aja fora da conversa sem aprovação explícita do usuário.

Tem 763 caracteres; em 2026-11-04, 688 couberam sem corte e o limite não é documentado. Se for cortada, o modelo não vai funcionar: avise antes de publicar.

## 3. Publique o modelo

1. Envie ao Bot: "Crie um modelo de você mesmo que eu possa compartilhar com outra pessoa, com a descrição atual." Se o Bot já tinha um modelo, use o ícone de compartilhar no alto do painel do Bot e escolha "Atualizar modelo", que sincroniza a descrição nova.
2. No card, clique em "Ver detalhes" e em "Contexto": "Instruções" tem que mostrar a regra permanente. Se mostrar a descrição antiga, o modelo não pegou a mudança.
3. Clique em "Publicar" (o Bot não publica sozinho) e copie o link.

## 4. Teste o link

Abra o link, clique em "Add to Grok Bot" e, no Bot novo, mande só "oi" e depois "qual é a sua versão", sem pedir para ler nada. Ele tem que se apresentar como "Monteiro Lobato (IA)" e dizer a versão 1.6.0. Se responder genérico, não divulgue o link: use "Excluir modelo" no ícone de compartilhar.

## Versões novas

Quem importa recebe a versão que estiver no repositório na primeira conversa; depois disso, atualiza como a seção Atualizar de [install/grok-bot.md](grok-bot.md) explica. A descrição só precisa mudar quando a lista de arquivos da skill mudar; nesse caso, repita o passo 2 e "Atualizar modelo".
