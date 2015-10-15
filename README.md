# Android
- [Load Image](https://gist.github.com/Pierry/efe85c7a3ca3ef47cd9d) - Load image from path to ImageView
- [Colors resource](https://gist.github.com/Pierry/bd31cf7ab71225a963a9) - List of colors
- [IsConnected](https://gist.github.com/Pierry/48951570b23c42087112) - Verify connection state
- [Android Annotations](https://gist.github.com/Pierry/b3eab411c8865573b985) - Root and app buidle.gradle example
- [KSoap](https://gist.github.com/Pierry/7614007) - Basic class example
- [Font](https://gist.github.com/Pierry/5705640) - Change font family programmatically
- [AssertionConcern Java](https://gist.github.com/Pierry/943eaf507e3184a826ca) - Validation values
- [JitPack Config](https://gist.github.com/Pierry/86c70b3a084c1e451488) - JitPack basic config


# ASP.NET
- [AssertionConcern](https://gist.github.com/Pierry/1ebff90f088c1455453b) - Validation values
- [WebApiConfig](https://gist.github.com/Pierry/b5eea368e9452e69279a) - Basic Json formatters
- [Unity](https://gist.github.com/Pierry/49a54039fd7664263bd5) - Dependency Injection container (Web API, Owin, MVC)
- [Repository Pattern](https://gist.github.com/Pierry/b6ba424f3425305e4a6f) - Class base
- [AutoMapper Config](https://gist.github.com/Pierry/a0ca1ca54a7b63cf2104) - Implementation example

# Emmet (Zen Coding)
- [Operator ()](https://gist.github.com/Pierry/6784915)
- [Operator *](https://gist.github.com/Pierry/6784899)
- [Operator ^](https://gist.github.com/Pierry/6784887)
- [Operator +](https://gist.github.com/Pierry/6784875)
- [Operator >](https://gist.github.com/Pierry/6784867)

git bash
======================

### Stage this hunk [..]?
- y - stage this hunk
- n - do not stage this hunk
- q - quit; do not stage this hunk nor any of the remaining ones
- a - stage this hunk and all later hunks in the file
- d - do not stage this hunk nor any of the later hunks in the file
- g - select a hunk to go to
- / - search for a hunk matching the given regex
- j - leave this hunk undecided, see next undecided hunk
- J - leave this hunk undecided, see next hunk
- k - leave this hunk undecided, see previous undecided hunk
- K - leave this hunk undecided, see previous hunk
- s - split the current hunk into smaller hunks
- e - manually edit the current hunk
- ? - print help


Github Flow
======================

Há um branch master que é sempre deployável, tudo que está nesse branch já foi validado e está pronto para ir pra produção. As funcionalidades são desenvolvidas em feature branches, que são derivadas do master. As features branches podem conter múltiplos niveis de detalhamento, isso é recomendado caso mais de um desenvolvedor trabalhe na funcionalidade

### Passo a passo

Você tem uma funcionalidade para desenvolver, qual o passo a passo?

1.	Vá para o master e atualize o seu repositório local: git pull --rebase master
2.	Crie uma branch do master: git checkout -b hmg-my-fix (veja o padrão para nomeamento das branches logo abaixo)
3.	Faça o desenvolvimento, crie commits pequenos e concisos
4.	Atualize sua branch com o master todos os dias:
5.	Caso você trabalhe sozinho na branch, faça o rebase com o master:
        git checkout master
        git pull --rebase
        git checkout -b hmg-my-fix
        git rebase master
6.	Caso você trabalhe com outros desenvolvedores, apenas faça o merge do master: git merge master
7.	Ao terminar, publique sua branch e abra um PR (Pull-Request)  para code review: git push -u origin my-fix

### Nomeação de branches

Utilizar sempre -(dash) na separação das palavras.
O nome da sua branch deve refletir o seu conteúdo, não deixando de ser breve
Exemplos válidos: notifications, fix-user-email, elasticsearch-experiments, better-errors
Exemplos inválidos: fix_notificacoes, correcao-de_usuarios, fix_everything

### Commits

Os commits devem ser pacotes de modificações no código com poucos objetivos, portanto, deve-se sempre criar commits menores e mais descritivos.

### Dicas para um bom commit:

- O título do seu commit deve ser um sumário do que aquele commit está resolvendo
- Tente manter o título do commit em menos de 50 caracteres
- Sempre que possível, escreva uma descrição mais detalhada do seu commit

### Dicas gerais para utilizar o git

- Use o git bash
- Quando for criar um commit, utilize o comando git add -p para revisar tudo que irá entrar no commit, evite utilizar o git add .
- Utilize sempre do comando git commit -v para abrir um editor com as mudanças e para você poder descrever melhor o seu commit
- Nunca utilize git rebase em um branch que já está público e que há outro desenvolvedor trabalhando, isso vai causar um conflito muito chato
- Caso você tenha cometido algum erro ao manipular o git, não se desespere, tente utilizar o git reflog

