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

git init = *transforma a pasta criada em um repositório git*

git add “**nome do arquivo**” = *adiciona o arquivo no preparatório para o próximo commit*

git add . = *adiciona todos os arquivos faltantes ao preparatório para o commit*

echo “**nome do arquivo**” > .gitignore  = *ignora o arquivo na verificação do git status caso seja uma pasta “**nome da pasta/nome arquivo**”*
> [!CAUTION]
> para adicionar mais de um arquivo é necessário adicionar todos de uma vez usando quebra de linha e refazendo o mesmo comando para arquivos diferentes

echo “**nome do arquivo**” > .gitkeep  = *mantém o arquivo na verificação do git status caso seja uma pasta “**nome da pasta/nome arquivo**”*
> [!CAUTION]
> para adicionar mais de um arquivo é necessário adicionar todos de uma vez usando quebra de linha e refazendo o mesmo comando para arquivos diferentes

git commit -m “ **“descrição aqui”** ” = *commita os arquivos*

git push = *envia as alterações do repositório local para o repositório remoto*

git log = *mostra o histórico de commits*

rm -rf  “**nome do arquivo**” = *exclui arquivos pelo terminal*

git restore “**nome do arquivo**” = *restaura o arquivo para a versão anterior*

git commit --amend -m” “**descrição**” “ = *altera a descrição do último commit*

git reset –"**selecionar uma das opções**" "**hash do commit que deseja retornar**" = *desfaz commit*
- soft = *retorna para o commit selecionado e mantém os arquivos modificados em commits anteriores na área de preparação*
- mixed = *retorna para o commit selecionado e mantém os arquivos modificados em commits anteriores na área de trabalho*
- hard = *retorna para o commit selecionado e apaga os arquivos modificados posteriormente git reset **nome do arquivo.extensão** remove o arquivo da área de preparação*

git reset  “**pasta/nome do arquivo.extensão**” = *remove o arquivo dentro da pasta da área de preparação*

git restore –staged “**nome do arquivo.extensão ou pasta/nome do arquivo.extensão**” = *remove o arquivo da área de preparação*

touch “**nome do arquivo.extensão**” = *cria um arquivo*

touch “**nome do arquivo.extensão nome do arquivo.extensão**” = *cria vários arquivos*

touch “**pasta/nome do arquivo.extensão**” = *cria um arquivo dentro da pasta determinada*

touch “**pasta/nome do arquivo.extensão pasta/nome do arquivo.extensão**” = *cria vários arquivos dentro de uma pasta*

git pull = *atualiza o repositório local com arquivos e modificações no repositório remoto*

git checkout  “**nome da branch**” = *altera para a branch selecionada*

git checkout -b “**nome da branch**”  = *cria uma nova branch e altera da branch main para a criada*

git branch = *mostra todas as branchs do repositório*

git branch -v = *mostra o último commit de cada branch*

git branch -d “**nome da branch**” = *deleta a branch selecionada*

git merge “**nome da branch**” = *mescla a branch selecionada com a main*

git fetch “**nome da branch remota**” = *baixa a branch com as alterações mais recentes, mas não mescla os arquivos*

git diff “**nome da branch local e nome da branch remota**” = *compara as diferenças das duas branchs*

git stash = *arquiva modificações feitas, útil para criar uma nova branch sem aplicar as alterações feitas anteriormente*

git stash list = *mostra todas as modificações arquivadas*

git stash pop = *se você quiser trazer as alterações e excluir a alteração mais recente dessa pilha/lista*

git stash apply = *se você quiser manter essa alteração na lista para um uso posterior*

## Meios de autenticação

autenticar com o navegador te dá total acesso as branchs privadas do github.Em alguns momentos não é a opção adequada, sendo necessário fazer autenticação ou por Token ou chave SSH.

### Token:

abra o github > clicar na foto de perfil> settings>Developer Settings>Personal access Tokens> Tokens(classic) > generate new token> generate new token(classic):

Neste momento de um nome e selecione as permissões que esse token vai ter ao interagir com sua branch privada.

> [!CAUTION]
> DEPOIS DE CRIADO VOCÊ É REDIRECIONADO PARA UMA PÁGINA COM O TOKEN, CUIDADO ASSIM QUE FECHAR ESTA PÁGINA NÃO TERÁ MAIS ACESSO AO TOKEN.

depois é só inserir o token na aba token, ao tentar clonar um repositório

git config “**local**” credential.helper store = *salva a credencial do token*

abra o github > clicar na foto de perfil> settings>Developer Settings>Personal access Tokens> Tokens(classic) = *mostra os tokens criados e quando o mesmo expira*

caso não peça autenticação, você precisa remover as credenciais em “**Gerenciador de credenciais do Windows**” e remove as credenciais do github,

### Chave SSH: 

ssh-keygen -t ed25519 -c "**seu email**" =  *gera a chave*

Enter file in which to save the key (**caminho padrão da chave**):
Created directory '**caminho da chave**'. = *enter para salvar a chave no local padrão ou selecione onde salvar*

depois será pedido que se digite 2 vezes a frase senha  que o usuário escolheu


eval "$(ssh-agent -s)" = *starta o ssh agente*

depois é necessário passar o endereço da chave privada, caso seja o local padrão:

ssh-add ~/.ssh/id_ed25519

inserir a frase senha

abra o github > clicar na foto de perfil> settings>ssh and gpg keys>new ssh keys

Insira o nome da chave e escolha o tipo de chave.
retorne ao git bash para procurar a chave

cd ~/.ssh = *para acessar a pasta padrão das chaves ssh*

ls = *para listar arquivos*

cat “NomeChave.pub”  = *para listar o conteudo da chave publica*

volte ao site do github, e insira o conteúdo no campo onde você escolheu o nome da chave e o tipo

depois de adicionada é possível usar a chave ssh e a passphrase para clonar repositórios

git clone “ChaveSShAbaSSH.git” = *comando para clonar o repositório*

Caso seja a primeira vez, ele vai perguntar se quer mesmo clonar, digite yes e aperte enter.

logo em seguida vai pedir que entre com a sua passphrase, depois de digitar seu repositório vai ser clonada

## Modo Editor Site GitHub

na página inicial da seu repositório do github aperte a teclado "**.**" caso deseje abrir um editor de código parecido com o visual studio code para realizar alterações online no repositório

