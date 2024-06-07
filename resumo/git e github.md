# Git e GitHub

## Codigos e suas funções

CTRL+L  ou clear = *limpa o terminal*

git config = *lista todas a lista de configurações possíveis*

**local**
- “--global”  = *modifica configurações no usuário atual*
- “--system” = *modifica configurações na máquina para todos os usuários*
- “--local” = *modifica configurações em um repositório específico*

git config ”**local**“ user.name ”**nome**” = *define o nome de usuário*

git config ”**local**“ user.email ”**email**” = *define o email do usuário*

git config user.name e git config user.email = *retorna nome e email já configurados*

git config init.defaultBranch = *retorna o nome da branch padrão*

git config “**local**” init.defaultBranch “**nome**” = *altera o nome da branch padrão*

git config “**local**” --list = *retorna todas as configurações feitas*

git clone “**link**” = *clona o repositório do link*

git clone “**link**” “**nome**” = *clona o repositório do link, e altera o nome*

git clone “**link**” -- branch “**nome da branch**”  --single-branch = *clona a branch específica do repositório*

git remote -v = *mostra os repositórios remotos onde a branch está vinculada*

git config “**local**” credential.helper = *mostra se as credenciais foram armazenadas como temporárias(cache) ou permanentes(store)*

git config “**local**” credential.helper “**store ou cache**” = *altera o método de armazenamento*

git config “**local**” --show-origin “**nome do arquivo**” = *mostra onde está armazenado determinado arquivo*

git config “**local**” --show-origin credential.helper = *mostra onde está armazenado os arquivos de credenciais*

cat “**nome do arquivo**” = *abre o arquivo dentro do terminal*

mkdir “**nome da pasta**” = *cria pasta no terminal*

cd “**nome da pasta**”  - acessa a pasta criado

cd .. = *retorna uma pasta*

git remote add origin “**link do repositório**” = *vinculado o repositório local a um repositório remoto*

git status = *mostra como está o status dos arquivos*
> [!CAUTION]
> o comando git status ignora pastas vazias