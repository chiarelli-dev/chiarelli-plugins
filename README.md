# Chiarelli Plugins

Plugins gratuitos da Chiarelli Labs para Claude Code, Codex e Claude.ai. Hoje há um: **chiarelli-turno-invisivel**.

## Diagnóstico do Turno Invisível

Você descreve uma rotina manual da sua empresa (conciliação, cobrança, emissão de notas, fechamento, relatórios) e recebe um diagnóstico, o Custo de Operação Manual (COM) estimado em reais por mês e um próximo passo. A skill tem instruções em português, inglês e espanhol. O idioma da resposta varia por superfície: veja o estado da verificação abaixo.

- Para quem: gestores, administrativo e financeiro de pequenas e médias empresas.
- Custo: grátis. Não exige conta, chave nem configuração da Chiarelli Labs.
- O COM é o custo do tempo manual de hoje. Não é promessa de economia, de prazo nem de preço.

Exemplo de pedido:

> Toda semana a gente concilia o extrato do banco com o ERP, umas 6 horas somando o time todo, e faz a cobrança dos atrasados, mais 3 horas no total. Quem faz ganha entre R$ 3.500 e R$ 5.000.

## Estado da verificação

A skill foi testada em 2026-09-29, em uso real, por superfície:

- Claude.ai: testada por upload do .zip, com ressalvas de idioma (nos testes em inglês e espanhol a resposta veio em português).
- Claude Code: testada como skill de projeto.
- Codex CLI: testada como skill de projeto, com ressalvas (em 3 de 4 casos a resposta omitiu um link sugerido ou pediu menos informações). Idioma: o corpo principal da resposta veio no idioma solicitado, mas nos casos em inglês e espanhol foi observado um preâmbulo em português (causa não isolada).
- Codex IDE, Codex app e ChatGPT: não testados.
- A instalação e a remoção por este marketplace (comandos abaixo): ainda não verificadas após a publicação, em nenhuma superfície.

Se algo divergir da documentação atual da sua ferramenta, siga a documentação dela e nos avise.

## Instalação e remoção

### Claude Code

Instalar (ainda não verificado após a publicação):

```
/plugin marketplace add chiarelli-dev/chiarelli-plugins
/plugin install chiarelli-turno-invisivel@chiarelli-plugins
```

Remover (ainda não verificado após a publicação):

```
/plugin uninstall chiarelli-turno-invisivel@chiarelli-plugins
/plugin marketplace remove chiarelli-plugins
```

Os mesmos comandos existem no terminal: `claude plugin marketplace add`, `claude plugin install`, `claude plugin uninstall` e `claude plugin marketplace remove`.

### Codex CLI

Instalar (ainda não verificado após a publicação):

```
codex plugin marketplace add chiarelli-dev/chiarelli-plugins
codex plugin add chiarelli-turno-invisivel@chiarelli-plugins
```

Remover, em dois passos separados (ainda não verificado após a publicação):

```
codex plugin remove chiarelli-turno-invisivel@chiarelli-plugins
codex plugin marketplace remove chiarelli-plugins
```

### Claude.ai

Instalar a skill por upload do .zip (testado): baixe [downloads/diagnostico-turno-invisivel.zip](downloads/diagnostico-turno-invisivel.zip) deste repositório (botão "Download raw" do GitHub, ou a URL raw https://github.com/chiarelli-dev/chiarelli-plugins/raw/main/downloads/diagnostico-turno-invisivel.zip, que só vale depois da publicação deste repositório) e envie em Personalização > Habilidades > + Adicionar > Fazer upload de habilidade (em inglês: Customize > Skills > + Add > Upload skill). Exige a execução de código ativada. Remover: apagar a skill na mesma tela.

O .zip deste repositório é idêntico byte a byte ao que o site vai oferecer em https://chiarelli.dev/downloads/diagnostico-turno-invisivel.zip quando o site for publicado (esse link ainda não está no ar).

Instalar como plugin via marketplace no Claude.ai: não testado.

## Privacidade

- A skill só contém instruções. Não tem servidor MCP, hooks, scripts executáveis, credenciais, acesso automático à rede nem telemetria.
- O provedor de IA que você escolheu recebe o conteúdo da conversa. A skill não envia nada à Chiarelli Labs.
- Descreva a rotina com suas palavras. Evite nomes de pessoas, CPF/CNPJ, números de conta, senhas e arquivos.
- A skill não bloqueia tecnicamente o que você colar. Ela pede uma versão anonimizada, mas o cuidado é seu.

## Suporte

https://chiarelli.dev/contato

## Licença

MIT. Veja o arquivo LICENSE.

## English

Free plugins by Chiarelli Labs for Claude Code, Codex and Claude.ai. The Invisible Shift Diagnostic skill turns a description of a manual back-office routine into a diagnosis, an estimated Manual Operations Cost (COM) in BRL per month and a next step. The skill has instructions in Portuguese, English and Spanish. The reply language varies by surface: see the tested surfaces below. Instruction-only: no automatic network access, no telemetry. Tested on 2026-09-29: Claude.ai by .zip upload, with language caveats (in the English and Spanish tests the reply came in Portuguese); Claude Code as a project skill; Codex CLI as a project skill, with caveats (in 3 of 4 cases the reply left out a suggested link or asked for less information; the main body of the reply came in the requested language, but a Portuguese preamble was observed in the English and Spanish cases, cause not isolated). Codex IDE, Codex app and ChatGPT were not tested. Installing and removing through this marketplace are not verified yet after publication. Privacy: the AI provider you use receives the conversation; the skill sends nothing to Chiarelli Labs and does not technically block what you paste, so leave out names, tax IDs, account numbers, passwords and files. Install and remove commands are listed above. Support: https://chiarelli.dev/contato. License: MIT.

## Español

Plugins gratuitos de Chiarelli Labs para Claude Code, Codex y Claude.ai. La skill Diagnóstico del Turno Invisible convierte la descripción de una rutina manual de back-office en un diagnóstico, el Costo de Operación Manual (COM) estimado en reales por mes y un próximo paso. La skill tiene instrucciones en portugués, inglés y español. El idioma de la respuesta varía según la superficie: ve las superficies probadas más abajo. Solo instrucciones: sin acceso automático a la red y sin telemetría. Probada el 2026-09-29: Claude.ai por carga del .zip, con salvedades de idioma (en las pruebas en inglés y español la respuesta llegó en portugués); Claude Code como skill de proyecto; Codex CLI como skill de proyecto, con salvedades (en 3 de 4 casos la respuesta omitió un enlace sugerido o pidió menos información; el cuerpo principal de la respuesta llegó en el idioma solicitado, pero en los casos en inglés y español se observó un preámbulo en portugués, causa no aislada). Codex IDE, la app de Codex y ChatGPT no fueron probados. La instalación y la remoción por este marketplace aún no están verificadas tras la publicación. Privacidad: el proveedor de IA que usas recibe la conversación; la skill no envía nada a Chiarelli Labs y no bloquea técnicamente lo que pegues, así que evita nombres, CPF/CNPJ, números de cuenta, contraseñas y archivos. Los comandos de instalación y remoción están arriba. Soporte: https://chiarelli.dev/contato. Licencia: MIT.
