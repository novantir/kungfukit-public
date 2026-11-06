<!-- install/duet.md -->
# Instalar no Claude Duet

Montado a partir da documentação oficial consultada em 2026-10-25; ainda não testado numa conta real.

O Duet usa as skills e os plugins da sua conta Claude.

1. Em claude.ai, abra Customize > Plugins > Add > Add marketplace e informe `novantir/kungfukit-public`. Para repositório privado, conecte o GitHub e dê acesso ao app do Claude. Ative "Sync automatically".
2. Instale o plugin `writer-monteiro-lobato`. Alternativa: Customize > Skills > Upload com um zip da pasta `skills/writer-monteiro-lobato` (a pasta precisa ser o primeiro nível do zip).
3. No Duet, envie:

> Quando eu pedir "Monteiro Lobato (IA)", use a skill writer-monteiro-lobato e siga-a até eu encerrar o modo. Lembre-se disso. Na primeira vez, siga também a seção Versão e atualização da skill.

Para começar, peça "Monteiro Lobato (IA)": a persona se apresenta e sugere como seguir.

O Duet pede aprovação antes de enviar mensagens, pagar, assinar ou apagar; mantenha assim.

## Atualizar

Para saber se precisa atualizar, pergunte à persona qual versão ela tem e compare com a versão no README do plugin (esta é a 1.6.0).

Com "Sync automatically" ligado, o plugin acompanha o repositório. Sem ele, em Customize > Plugins, atualize o plugin (ou remova e instale de novo); no upload por zip, envie o zip da versão nova. Depois, no Duet: "A skill writer-monteiro-lobato foi atualizada; use a versão nova a partir de agora."
