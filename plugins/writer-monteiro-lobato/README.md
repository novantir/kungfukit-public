<!-- README.md -->
# Monteiro Lobato (IA): histórias, Brasil e leitura

Persona de IA inspirada nas obras de Monteiro Lobato, em domínio público; não oficial, sem afiliação nem endosso de herdeiros ou entidades ligadas ao nome, não é a pessoa nem fala em nome dela. Conta e inventa histórias no estilo de Monteiro Lobato, para crianças e adultos, conversa sobre o Brasil das crônicas dele e ensina leitura e escrita, a partir das obras dele publicadas até 1930 (Urupês, Cidades Mortas, Negrinha, A Menina do Narizinho Arrebitado e outras). A primeira persona em português desta coleção.

Versão **1.6.0**, categoria `writer`, idioma português. Piloto por curadoria assistida; qualidade no bot real ainda não avaliada.

## Instalar no seu bot

| Bot | Como |
| --- | --- |
| Grok Bot | [install/grok-bot.md](install/grok-bot.md): envie o prompt do guia ao Grok Bot principal, que busca os arquivos pelo GitHub e cria o Bot da persona; ou crie o Bot você mesmo e mande a mensagem de instalação. |
| Dots (ChatGPT) | [install/dots.md](install/dots.md): plugin do repositório ou mensagem de instalação. |
| Claude Duet | [install/duet.md](install/duet.md): plugin pela loja do repositório, que também vale para claude.ai. |
| Loja do Grok Bot | [install/grok-template.md](install/grok-template.md): regra permanente na descrição do Bot e publicação como modelo; só personas de domínio público. |
| Claude Code | `/plugin install writer-monteiro-lobato --marketplace novantir/kungfukit-public` |

Em qualquer bot com campo de instruções, cole o conteúdo de `skills/writer-monteiro-lobato/SKILL.md` e anexe os arquivos de `skills/writer-monteiro-lobato/references/`. No Grok Bot, a leitura pelo GitHub e a criação pelo Grok Bot principal foram testadas em contas reais em 2026-10-26 e 2026-10-27, com outras personas do KungfuKit (esta ainda não foi testada num bot); Dots e Duet seguem a documentação oficial consultada em 2026-10-25, sem teste.

Depois de instalada, a persona se apresenta e sugere como começar:

- Conte uma história no estilo dele, com bichos que falam e uma menina curiosa.
- Recontar um conto de Urupês, Cidades Mortas ou Negrinha e conversar sobre ele.
- Conversar sobre o Brasil que ele criticou: o Jeca Tatu, as cidades mortas, a burocracia.
- Ajudar a escrever um texto claro, do jeito que ele defendia.

## Arquivos

| Arquivo | Uso |
| --- | --- |
| `skills/writer-monteiro-lobato/SKILL.md` | Instruções da persona: identificação como IA, limites de ação e regras. |
| `skills/writer-monteiro-lobato/references/knowledge.md` | Notas de conhecimento com fontes e datas. |
| `skills/writer-monteiro-lobato/references/evidence.md` | Regras com evidências, trechos literais das obras e limitações; a persona o usa para citar. |
| `install/` | Mensagens de instalação para Grok Bot, Dots e Duet. |
| `provenance/persona.json` | Pacote curado completo: regras, trechos de evidência e manifesto. |
| `sources.json` | Fontes usadas, com datas e licença conhecida. |
| `package-manifest.json` | Versão, alvos, validação e hashes. |

## O que esta persona faz e não faz

Faz: conta e inventa histórias no estilo de Monteiro Lobato, para crianças e adultos; reconta as histórias das obras dele até 1930 (Narizinho, os contos de Urupês, Cidades Mortas e Negrinha, as crônicas); conversa sobre o Brasil que ele retratou e criticou, com as posições dele datadas; e ensina leitura e escrita com a clareza e o humor dele. Responde no idioma de quem escreve.

Não faz: não fala como Monteiro Lobato nem inventa frases dele; entre aspas, só trechos literais do pacote, com obra e ano. Não representa o autor nem os herdeiros. Não adota o racismo que aparece em várias obras: quando perguntam, cita o texto com contexto histórico e diz com clareza que é racismo. O Sítio do Picapau Amarelo publicado de 1931 em diante fica fora do pacote.

## Fontes utilizadas

Obras de Monteiro Lobato (1882–1948) em domínio público, publicadas até 1930, em edições da época:

- Urupês (1918), 3ª edição, Wikisource
- Cidades Mortas (1919), 3ª edição, Wikisource
- A Menina do Narizinho Arrebitado (1920), fac-símile no archive.org (ameninadonarizinho), só o texto de Lobato
- Negrinha (1920), 4º milheiro, Wikisource
- A Onda Verde (1921), 2ª edição, Wikisource
- Mundo da Lua (1923), Wikisource
- O Macaco que se fez Homem (1923), Wikisource
- Jéca Tatuzinho (1924), archive.org (JecaTatuzinho1924)
- O Choque das Raças (1926), Wikisource
- Mister Slang e o Brasil (1927), Wikisource

## Estado da validação

19 regras e 192 notas de conhecimento (resumos de histórias e posições datadas). Cada regra tem evidências literais em pelo menos duas obras; as citações têm no máximo 40 palavras. A base do domínio público foi conferida pelo motor (morte há mais de 70 anos, obras publicadas há mais de 95). Seis contos e capítulos foram sorteados antes da leitura e reservados para o teste de fidelidade, e oito para desenvolvimento. Sem avaliação em bot real nem chamada paga de modelo.
