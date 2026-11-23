# Controled para o Claude

Plugin do [Controled](https://controled.com.br) para o Claude (claude.ai, app do Claude, Cowork e
Claude Code). Ele junta o conector do Controled a uma skill que ensina o Claude a operar a rede de
telas de LED e totens da sua empresa: telas e players, anunciantes, contratos, campanhas,
programação institucional, mídias, layouts com notícias e clima, criador de vídeo, relatórios e
diagnósticos.

O plugin fica em [`plugins/controled`](plugins/controled), com o que ele faz, como usar e que dados
envia.

## Instalar

- **Claude.ai, app do Claude e Cowork**: em Personalizar › Plugins › Adicionar › Adicionar
  marketplace, informe `igorgaffuri/controled-claude-plugin` e instale o plugin Controled.
- **Claude Code**, dentro da sessão:

  ```
  /plugin marketplace add igorgaffuri/controled-claude-plugin
  /plugin install controled@controled
  ```

  Ou no terminal: `claude plugin install controled --marketplace igorgaffuri/controled-claude-plugin`.

Depois, conecte o conector do Controled pela aba de conectores do plugin, com a sua conta do
Controled.

## Antes de conectar

- Ser membro ativo do painel de uma organização no Controled, com qualquer cargo, e com a
  verificação em duas etapas ativa. O Claude faz só o que o seu cargo permite no painel.
- O interruptor **Conector da organização** ligado em Perfil › Conectores de IA, no painel do
  Controled. Quem liga é um administrador (cargo de nível 50 ou mais), uma vez para toda a
  organização.

Na autorização, numa tela só, o Claude recebe leitura e edição, e as permissões sensíveis (gerar
vídeo, relatório por e-mail, equipe, exclusões, reiniciar a máquina de uma tela) aparecem
desmarcadas para você marcar as que vai usar. Se depois uma ação precisar de uma que ficou
desmarcada, o Controled pede só aquela.

## Atualizar

Quem adicionou o marketplace recebe as versões novas pela sincronização do Claude. No Claude Code:
`/plugin marketplace update controled`.

## Suporte

- WhatsApp: [+55 47 99752-0288](https://wa.me/5547997520288)
- E-mail: suporte@controled.com.br
- Documentação da API e Termos do Conector: https://controled.com.br/docs/api

Este repositório é uma cópia publicada; o plugin é mantido junto com o código do Controled.
Licença: [LICENSE](plugins/controled/LICENSE).
