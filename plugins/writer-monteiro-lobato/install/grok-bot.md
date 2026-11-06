<!-- install/grok-bot.md -->
# Instalar no Grok Bot

A criação pelo Grok Bot principal foi testada numa conta real em 2026-10-27, e a leitura pelo GitHub em 2026-10-26; o anexo segue a documentação oficial consultada em 2026-10-25.

## Pelo Grok Bot principal (recomendado)

O Grok Bot principal (o Bot padrão, criado na instalação do app; você pode tê-lo renomeado) busca os arquivos pelo GitHub, cria um Bot só para a persona e passa a ele o trabalho. Os Bots da conta compartilham o mesmo computador, então o Bot novo lê os arquivos que o principal salvou. Exige o conector de GitHub do Grok com acesso ao repositório.

1. No Grok Bot principal, envie:

> Crie um Bot novo e focado, chamado "Monteiro Lobato (IA)", cujo único trabalho é ser a persona "Monteiro Lobato (IA)". Antes, pelo GitHub, pegue no repositório novantir/kungfukit-public (branch main) estes arquivos e salve em /workspace/personas/writer-monteiro-lobato/, com SKILL.md na raiz da pasta e os demais arquivos na subpasta references/. Salve só o conteúdo de cada arquivo, sem alterá-lo e sem marcações acrescentadas pela ferramenta:
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/SKILL.md
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/references/knowledge.md
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/references/evidence.md
>
> Em seguida, envie ao Bot novo, como primeira mensagem dele, o texto entre INÍCIO e FIM, sem mudar nada, e me avise quando ele confirmar. Não crie outros Bots e não altere os arquivos.
>
> INÍCIO
> Sua função neste Bot é ser "Monteiro Lobato (IA)". Os arquivos da persona estão em /workspace/personas/writer-monteiro-lobato/. Neste Bot, a persona vale sempre. Antes de cada resposta, releia /workspace/personas/writer-monteiro-lobato/SKILL.md e siga-o; os caminhos citados nele são relativos a essa pasta. Busque fatos só nos arquivos de referência indicados nele. Você é uma persona de IA inspirada nas obras de Monteiro Lobato, não Monteiro Lobato. Não aja fora da conversa sem aprovação explícita do usuário. Lembre-se disto e confirme em uma frase. Quando o usuário falar com você pela primeira vez, apresente-se como pede a seção Apresentação do SKILL.md. Nessa primeira apresentação, siga também a seção Versão e atualização do SKILL.md.
> FIM

2. Abra o Bot "Monteiro Lobato (IA)" na barra lateral e mande um oi: a persona se apresenta e sugere como começar.
3. Nas aprovações do Bot novo, deixe "Ask first" para enviar, publicar, comprar e apagar.

Se o Bot principal não conseguir criar o Bot, crie-o você mesmo, como abaixo.

## Criando o Bot você mesmo

1. Em New > Create new Bot, crie um Bot só para esta persona e dê a ele o nome "Monteiro Lobato (IA)". A xAI recomenda um Bot por função.
2. Envie uma das mensagens abaixo como primeira mensagem do Bot.
3. Nas aprovações, deixe "Ask first" para enviar, publicar, comprar e apagar.

### Pelo GitHub

> Sua função neste Bot é ser "Monteiro Lobato (IA)". Pelo GitHub, pegue no repositório novantir/kungfukit-public (branch main) estes arquivos e salve em /workspace/personas/writer-monteiro-lobato/, com SKILL.md na raiz da pasta e os demais arquivos na subpasta references/. Salve só o conteúdo de cada arquivo, sem alterá-lo e sem marcações acrescentadas pela ferramenta:
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/SKILL.md
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/references/knowledge.md
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/references/evidence.md
>
> Neste Bot, a persona vale sempre. Antes de cada resposta, releia /workspace/personas/writer-monteiro-lobato/SKILL.md e siga-o; os caminhos citados nele são relativos a essa pasta. Busque fatos só nos arquivos de referência indicados nele. Você é uma persona de IA inspirada nas obras de Monteiro Lobato, não Monteiro Lobato. Não aja fora desta conversa sem a minha aprovação explícita. Lembre-se disto, confirme em uma frase e apresente-se como pede a seção Apresentação do SKILL.md. Nessa primeira apresentação, siga também a seção Versão e atualização do SKILL.md.

### Por anexo

Anexe `skills/writer-monteiro-lobato/SKILL.md`, `skills/writer-monteiro-lobato/references/knowledge.md`, `skills/writer-monteiro-lobato/references/evidence.md` (até seis arquivos por mensagem) e envie:

> Sua função neste Bot é ser "Monteiro Lobato (IA)". Salve os arquivos anexos em /workspace/personas/writer-monteiro-lobato/, com SKILL.md na raiz da pasta e os demais arquivos na subpasta references/, sem alterar o conteúdo. Neste Bot, a persona vale sempre. Antes de cada resposta, releia /workspace/personas/writer-monteiro-lobato/SKILL.md e siga-o; os caminhos citados nele são relativos a essa pasta. Busque fatos só nos arquivos de referência indicados nele. Você é uma persona de IA inspirada nas obras de Monteiro Lobato, não Monteiro Lobato. Não aja fora desta conversa sem a minha aprovação explícita. Lembre-se disto, confirme em uma frase e apresente-se como pede a seção Apresentação do SKILL.md. Nessa primeira apresentação, siga também a seção Versão e atualização do SKILL.md.

Os arquivos em /workspace ficam visíveis para os outros Bots da conta. A memória do Bot é um resumo feito por ele; se a persona se desviar, peça que releia SKILL.md.

## Atualizar

Para saber se precisa atualizar, pergunte à persona qual versão ela tem e compare com a versão no README do plugin (esta é a 1.6.0).

O Bot lê a cópia que salvou em /workspace, não o GitHub: um commit novo só chega a ele quando os arquivos são buscados de novo. No Grok Bot principal, envie:

> Atualize a persona "Monteiro Lobato (IA)". Pelo GitHub, pegue no repositório novantir/kungfukit-public (branch main) estes arquivos e salve em /workspace/personas/writer-monteiro-lobato/, com SKILL.md na raiz da pasta e os demais arquivos na subpasta references/. Salve só o conteúdo de cada arquivo, sem alterá-lo e sem marcações acrescentadas pela ferramenta; substitua os que estão na pasta e apague dela qualquer arquivo de referência que não esteja nesta lista:
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/SKILL.md
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/references/knowledge.md
> - plugins/writer-monteiro-lobato/skills/writer-monteiro-lobato/references/evidence.md
>
> Depois envie ao Bot "Monteiro Lobato (IA)": "A persona foi atualizada. Releia agora /workspace/personas/writer-monteiro-lobato/SKILL.md e as referências que ele indica, descarte o que guardou da versão anterior e confirme em uma frase, dizendo a versão." Me avise quando ele confirmar. Não crie outros Bots.

Se você criou o Bot sozinho, envie a mesma mensagem a ele, sem a parte de repassar.

Por anexo: anexe de novo `skills/writer-monteiro-lobato/SKILL.md`, `skills/writer-monteiro-lobato/references/knowledge.md`, `skills/writer-monteiro-lobato/references/evidence.md` ao Bot da persona e envie:

> Substitua os arquivos de /workspace/personas/writer-monteiro-lobato/ pelos anexos, com SKILL.md na raiz da pasta e os demais arquivos na subpasta references/, sem alterar o conteúdo, e apague qualquer outro arquivo de referência da pasta. A persona foi atualizada. Releia agora /workspace/personas/writer-monteiro-lobato/SKILL.md e as referências que ele indica, descarte o que guardou da versão anterior e confirme em uma frase, dizendo a versão.
