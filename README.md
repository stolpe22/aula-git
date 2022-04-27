# aula-git
Projeto de teste usado no curso do prof. Nelio Alves

Anotações de comandos git

git status
=mostra o que tem pra commitar e o que foi commitado

git add .
=prepara os arquivos modificados para commit

git commit -m "message"
=commita os arquivos preparados com a mensagem descrita no -m

git log
=mostra um log dos commits feitos

git log --oneline
=mostra um log resumido dos commits feitos

git clean -df
git checkout -- .
=desfaz mudanças feitas não commitadas, retornando ao status original do último commit

git reset --soft HEAD~1
=desfaz o último commit e mantém as alterações no gatilho

git reset --hard HEAD~1
=desfaz o último commit e exclui também as alterações no código fonte

git checkout 6346c7e
=precisa estar sem alterações pendentes para commit. Utilizado para verificar como estava o codigo no commit referenciado, sem alterar nada nas alterações que estão sendo feitas no momento.

git checkout branch
=direciona de volta para o que está sendo feito no momento após dado um (git checkout k553cd). coloque o nome da branch, exemplo: master

git remote add origin <URI do repositório remoto>
=associa repositório local ao repositório remoto, dando o apelido de "origin" a ele

git remote set-url origin <URI do repositório remoto>
=associa o repositório local a um outro repositório remoto, porém mantendo o mesmo apelido

git push -u origin master
=para primeiro push

git push
=se ja usado a opção -u, nas próximas vezes só dar o push

git clone <URI do repositório>
=Clona o repositório para maquina local com os historicos de commit
!apenas download não copia histórico

git pull origin master
=para dar pull em repositorio git

git diff nomearquivo.ext
Mostra as diferenças do arquivo no novo estado para o estado antigo, linhas adicionadas e excluidas, por exemplo


