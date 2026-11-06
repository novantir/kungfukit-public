<!-- install/dots.md -->
# Instalar no Dots (ChatGPT)

Montado a partir da documentação oficial consultada em 2026-10-25; ainda não testado numa conta real.

## Pelo plugin (preferível)

O repositório traz o plugin em formato Codex (`.codex-plugin/plugin.json`) e a skill em `skills/writer-monteiro-lobato/`. No app de desktop do ChatGPT, adicione a loja do repositório (`codex plugin marketplace add novantir/kungfukit-public`), reinicie o app e instale "Monteiro Lobato (IA): histórias, Brasil e leitura" no diretório de plugins. A documentação não diz se o Dot usa skills de plugins; confirme pedindo que ele liste as skills disponíveis.

## Pela conversa (alternativa)

Envie ao seu Dot a mensagem abaixo e, em seguida, cole o conteúdo de `skills/writer-monteiro-lobato/SKILL.md`, `skills/writer-monteiro-lobato/references/knowledge.md`, `skills/writer-monteiro-lobato/references/evidence.md`.

> Quando eu pedir "Monteiro Lobato (IA)", use as instruções e referências que vou enviar até eu encerrar o modo. Guarde-as nas suas notas sem resumir as regras. Você é uma persona de IA inspirada nas obras de Monteiro Lobato, não Monteiro Lobato. Não aja fora da conversa sem a minha aprovação. Confirme em uma frase. Na primeira vez em que eu pedir a persona, siga também a seção Versão e atualização do SKILL.md.

## Regras personalizadas sugeridas

Em Configurações > Personalização > Permissões > Regras personalizadas: "perguntar antes" para enviar mensagens e publicar; "passar para mim" para compras e exclusões.

Para começar, peça "Monteiro Lobato (IA)": a persona se apresenta e sugere como seguir.

## Atualizar

Para saber se precisa atualizar, pergunte à persona qual versão ela tem e compare com a versão no README do plugin (esta é a 1.6.0).

Pelo plugin: atualize a loja do repositório no diretório de plugins do app de desktop (ou desinstale e instale o plugin de novo) e reinicie o app. Pela conversa: envie "Vou mandar a versão nova da persona Monteiro Lobato (IA); substitua nas suas notas a anterior, sem resumir as regras." e cole de novo o conteúdo de `skills/writer-monteiro-lobato/SKILL.md`, `skills/writer-monteiro-lobato/references/knowledge.md`, `skills/writer-monteiro-lobato/references/evidence.md`.
