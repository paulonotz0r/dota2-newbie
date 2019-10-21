# Contribuições


### Por onde começar?

**1.** Faça o _fork_ do projeto.

**2.** [Entenda o fluxo](#fluxo).


### Fluxo


**1.** Faça referência ao repositório oficial após o _fork_

* Passos
    - Crie uma pasta e abra com o editor que preferir (_vim_, _sublime_, *_vscode_*)
    - Dê um fork no repositorio original https://github.com/paulonotz0r/dota2-newbie.
    - Apos o fork, o repositorio estará salvo no seu github, então dê um git clone usando o terminal no diretorio da pasta criada `git clone https://github.com/usuario/dota2-newbie`
    - Se você precisar fazer mais alguma alteração no mesmo repositório no futuro, mas já tem outras colaborações no repositório original é necessario sicronizar o projeto

```
git remote add upstream https://github.com/paulonotz0r/dota2-newbie.git
git fetch upstream
git merge upstream/master
```

**2.** Antes de iniciar o processo de contribuição, crie uma nova branch para fazer suas alterações.

Só alguns exemplos:

- Para tradução: `git checkout -b traducao`
- Para erros: `git checkout -b correcao`

> Use qualquer nome que seja coerente com a contribuição que está sendo feita.


**3.** Após realizar as alterações, é hora de fazer um commit com uma mensagem coerente do que foi feito. Exemplo:

```
git add --all
git commit -am ‘Adiciona tradução/melhoria linha/linhas Y’
git push origin traducao
```

**4.** Envie um _Pull Request_ com as alterações feitas, fazendo referência para o `master` do repositório oficial.

**5.** Sua contribuição será analisada.

Após o merge:

- Delete a branch utilizada:

```
git checkout master
git push origin :traducao
git branch -D traducao
```

- Atualize seu repositório com o repositório oficial:

```
git fetch upstream
git rebase upstream/master
git push -f origin master
```


Obrigado newbas! :heart: