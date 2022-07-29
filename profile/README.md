# [Fluxo de Desenvolvimento](#fluxo-de-desenvolvimento):
1) [Verificar se a branch atual é a master](#step-1). 
   O git bash indica a branch atual entre parênteses em azul ao lado do caminho do repositório;
2) Caso não esteja na branch master realizar o checkout para ela com o comando:
 - `$ git checkout master`;
3) Verificar se a branch master está atualizada com o comando:
 - `$ git pull`;
4) Criar uma nova branch a partir da master com o comando `$ git checkout -b <nome-da-nova-branch>`;
 - Exemplo: `$ git checkout -b bugfix/os-0123456`;
5) O padrão adotado para os nomes das branches é `bugfix/os-<numero-da-os>` para correção e `feature/os-<numero-da-os>` para alteração ou funcionalidade nova;
6) Preparar para commit os arquivos criados, alterados ou excluídos com os comandos: 
 - `$ git add <nome-do-arquivo>` para cada arquivo;
 - `$ git add -A` para todos os arquivos;
7) Criar o commit com o comando `$ git commit -m "Mensagem do commit."`;
 - Exemplo: `$ git commit -m "Corrige a listagem de produtos."`;
8) O padrão adotado para os commits inicia a mensagem com um verbo no presente do indicativo, exemplos: 
 - `"Cria formulário para devolução de compra"`
 - `"Adiciona filtro de cor no relatório de vendas"`;
9) Subir os commits para o github com o comando `$ git push`; 
10) Caso a branch ainda não exista no repositório remoto (github), será necessário subir a referência com o comando `$ git push -u origin <nome-da-branch>`;
11) Criar uma pull request (PR) no github, apontando para a branch master, com pelo menos um revisor;
12) O padrão adotado para o título da PR inicia com `[OS <numero-da-os>] O que foi feito para a os.`; 
 - Exemplo: `[OS 0123456] Cria formulário para devolução de compra`;
13) O padrão adotado para a descrição da PR indica o que foi feito para a OS mais detalhadamente e indica alguns possíveis teste que podem ser feitos para aprovar a PR;
14) Voltar ao passo [1](#fluxo-de-desenvolvimento);

## [Drive](https://drive.google.com/drive/folders/189BioREeAycEjbd5Llr-9G79jthT5zOq)
 - [Como usar o GIT](https://drive.google.com/drive/folders/10YxtwU9rvXXUVeU2qQHJGZ_ait4T4FFz)

## Padrão de Commits:

### Conventional Commits
- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
- [Commitizen](https://commitizen-tools.github.io/commitizen/)
- [Hook for Conventional Commits](https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13)
- [Husky](https://github.com/typicode/husky)
