# Ativação do Modo Pro (código de uso único = 1 aparelho)

O app já vem com o Modo Pro ligado ao mesmo script do app original (`pro-config.js`, campo `scriptUrl`) e com `app: 'fingerstyle'`.

**Se o script do app original aceita qualquer nome em `app`** (ou você quer usar o mesmo), nada mais é preciso:
basta cadastrar os códigos na planilha dele, com `fingerstyle` na coluna do app (se existir).

**Se preferir um script só deste app** (ou o antigo não aceitar o nome novo):
1. Crie uma planilha no Google Drive e renomeie a aba para `Codigos`.
2. Linha 1: `codigo | app | dispositivo | status | ativado_em | anotacao`.
3. Em Extensões → Apps Script, apague tudo e cole o `Code.gs` desta pasta.
4. Implantar → Nova implantação → App da Web → Executar como: **você** · Quem tem acesso: **Qualquer pessoa** → Implantar.
5. Copie o endereço que termina em `/exec` e cole em `scriptUrl` no `pro-config.js`.
6. Para vender: escreva um código novo na coluna A (ex.: `PRO-AB12-CD34`) e, na coluna B, `fingerstyle`. Deixe C, D e E vazias.
   Para cancelar um código: escreva `bloqueado` na coluna D.

Depois de qualquer mudança no script, faça **Implantar → Gerenciar implantações → editar → Nova versão**.
