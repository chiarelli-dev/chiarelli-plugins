# chiarelli-turno-invisivel

Diagnóstico do Turno Invisível (pt), Invisible Shift Diagnostic (en), Diagnóstico del Turno Invisible (es). Skill gratuita da Chiarelli Labs: você descreve uma rotina manual da sua empresa e recebe um diagnóstico, o Custo de Operação Manual (COM) estimado em reais por mês e um próximo passo.

## Requisitos

- Uma das superfícies: claude.ai, Claude Code ou Codex.
- Nenhuma conta, chave ou configuração extra da Chiarelli Labs.

## Onde baixar o .zip

O arquivo `diagnostico-turno-invisivel.zip` fica na pasta `downloads/` do repositório público chiarelli-dev/chiarelli-plugins: [../../downloads/diagnostico-turno-invisivel.zip](../../downloads/diagnostico-turno-invisivel.zip). O link relativo só vale depois da publicação do repositório e a partir deste README dentro dele.

## Instalação e remoção

Estado da verificação por superfície:

- claude.ai: a skill foi testada por upload do .zip, com ressalvas de idioma (nos testes em inglês e espanhol a resposta veio em português).
- Claude Code: a skill foi testada como skill de projeto.
- Codex CLI: a skill foi testada como skill de projeto, com ressalvas (em 3 de 4 casos a resposta omitiu um link sugerido ou pediu menos informações). Idioma: o corpo principal da resposta veio no idioma solicitado, mas nos casos em inglês e espanhol foi observado um preâmbulo em português (causa não isolada).
- Codex IDE, Codex app e ChatGPT: não testados.
- A instalação e a remoção por plugin local ou marketplace ainda não foram testadas em nenhuma superfície.

Se algo divergir da documentação atual da sua ferramenta, siga a documentação dela e nos avise.

### claude.ai

- Instalar: Personalização > Habilidades > + Adicionar > Fazer upload de habilidade (em inglês: Customize > Skills > + Add > Upload skill; os nomes podem variar conforme o idioma da interface), e enviar o arquivo `diagnostico-turno-invisivel.zip`. Exige a execução de código ativada; em planos Enterprise vale a política do Owner.
- Remover: apagar a skill na mesma tela.

### Claude Code

- Instalar (ainda não verificado): adicionar esta pasta como plugin local, conforme a documentação atual do Claude Code.
- Remover (ainda não verificado): `claude plugin uninstall chiarelli-turno-invisivel`.

### Codex

- Instalar (ainda não verificado): colocar esta pasta em um marketplace local de plugins, conforme a documentação atual do Codex.
- Remover (ainda não verificado): desinstalar pelo gerenciador de plugins do Codex.

## Privacidade

- A skill só contém instruções. Não tem servidor MCP, hooks, scripts executáveis, credenciais, acesso automático à rede nem telemetria.
- O provedor de IA que você escolheu recebe o conteúdo da conversa. A skill não envia nada à Chiarelli Labs.
- Descreva a rotina com suas palavras. Evite nomes de pessoas, CPF/CNPJ, números de conta, senhas e arquivos.
- A skill não bloqueia tecnicamente o que você colar. Ela pede uma versão anonimizada, mas o cuidado é seu.

## Suporte

https://chiarelli.dev/contato
