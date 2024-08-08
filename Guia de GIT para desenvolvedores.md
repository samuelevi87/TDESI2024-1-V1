## 

Guia Completo de Git para Desenvolvedores Iniciantes

### **1\. Tabela de Comandos Git Essenciais**

| Fluxo de Trabalho | Passo | Comando Git | Parâmetros | Explicação | Exemplo Prático |
| :---- | :---- | :---- | :---- | :---- | :---- |
| Iniciar um novo projeto | Criar repositório local | git init |  | Inicializa um novo repositório Git no diretório atual. | git init meu-projeto |
|  | Adicionar arquivos ao staging area | git add . |  | Adiciona todos os arquivos modificados ao staging area. | git add . |
|  | Commitar as alterações | git commit \-m "Mensagem do commit" |  | Cria um snapshot das alterações adicionadas ao staging area. | git commit \-m "Primeira versão do projeto" |
| Trabalhar em uma nova funcionalidade | Criar um novo branch | git branch nova-funcionalidade |  | Cria um novo branch a partir do branch atual. | git branch nova-funcionalidade |
|  | Mudar para o novo branch | git checkout nova-funcionalidade |  | Muda para o branch recém-criado. | git checkout nova-funcionalidade |
|  | Adicionar e commitar as alterações | git add . e git commit \-m "..." |  | Adiciona e commita as alterações no novo branch. | git add . e git commit \-m "Implementando nova funcionalidade" |
| Colaborar com outros desenvolvedores | Clonar um repositório remoto | git clone https://github.com/usuario/repositorio.git |  | Cria uma cópia local de um repositório remoto. | git clone https://github.com/facebook/react |
|  | Adicionar um remote | git remote add origin https://github.com/usuario/repositorio.git |  | Adiciona um remote com o nome "origin" para o repositório remoto. | git remote add origin https://github.com/meu-usuario/meu-projeto.git |
|  | Pushar as alterações para o remote | git push origin nova-funcionalidade |  | Envia as alterações do branch local para o branch remoto. | git push origin nova-funcionalidade |
| Resolver conflitos de merge | Mesclar um branch | git merge outro-branch |  | Mescla as alterações de outro branch no branch atual. | git merge main |
|  | Resolver conflitos manualmente | Abrir os arquivos com conflito e editar manualmente. |  | Editar os arquivos com marcadores de conflito (\<\<\<, \>\>\>) para resolver as diferenças. |  |
|  | Adicionar e commitar a resolução | git add . e git commit \-m "..." |  | Adicionar os arquivos resolvidos e commitar as alterações. | git add . e git commit \-m "Resolvendo conflito" |
| Preparar uma release | Criar uma tag | git tag v1.0.0 |  | Cria uma tag para marcar uma versão específica. | git tag v1.0.0 |
|  | Pushar a tag para o remote | git push origin v1.0.0 |  | Envia a tag para o repositório remoto. | git push origin v1.0.0 |

**Lembre-se:** A melhor forma de aprender Git é praticando. Experimente os comandos em seus próprios projetos e consulte a documentação oficial para mais informações.

## 

2\. Guia SOS para Git

| Problema Comum | Comando(s) para Solução | Explicação da Solução | Exemplo de uso |
| :---- | :---- | :---- | :---- |
| Desfazer o último commit | git reset \--soft HEAD\~ | Reverte o último commit, mas mantém as alterações no staging area. | git reset \--soft HEAD\~ |
| Reverter alterações em um arquivo específico | git checkout HEAD \-- arquivo.txt | Reverte as alterações em um arquivo específico para o último commit. | git checkout HEAD \-- index.html |
| Corrigir uma mensagem de commit errada | git commit \--amend | Edita a mensagem do último commit. | git commit \--amend |
| Recuperar um arquivo deletado acidentalmente | git restore \--source=HEAD arquivo.txt | Restaura um arquivo deletado para o estado do último commit. | git restore \--source=HEAD imagem.jpg |
| Mudar de branch preservando alterações não commitadas | git stash | Salva as alterações não commitadas temporariamente. | git stash |

### **3\. Boas Práticas de Git**

* **Commits pequenos e descritivos:** Faça commits frequentes com mensagens claras e concisas sobre as alterações realizadas.  
* **Branches temáticas:** Utilize branches para desenvolver funcionalidades específicas, mantendo o branch principal limpo.  
* **Rebase com cuidado:** O rebase pode simplificar o histórico, mas use-o com cautela, especialmente em projetos colaborativos.  
* **Utilize tags:** Marque versões importantes do projeto com tags para facilitar o gerenciamento de releases.  
* **Faça backups regulares:** Além do controle de versão do Git, é recomendado fazer backups regulares do repositório completo.

### **4\. Comparação: Linha de Comando vs. Ferramentas Gráficas**

| Comando Git | Equivalente em Ferramentas Gráficas |
| :---- | :---- |
| git status | Verificar status do repositório |
| git add . | Adicionar arquivos ao staging area |
| git commit \-m "mensagem" | Commitar alterações |
| git branch | Criar, listar ou excluir branches |
| git checkout | Mudar de branch |
| git merge | Mesclar branches |
| git pull | Atualizar repositório local |
| git push | Enviar alterações para o repositório remoto |

**Nota:** As opções disponíveis nas ferramentas gráficas podem variar.

### **5\. Dicas de Produtividade**

* **Utilize aliases:** Crie aliases para comandos Git frequentemente usados, como git st para git status.  
* **Configure o editor padrão:** Defina seu editor de texto favorito como o editor padrão para mensagens de commit.  
* **Use hooks Git:** Automatize tarefas com hooks Git, como verificações de código antes do commit.  
* **Explore ferramentas de visualização:** Utilize ferramentas como git log \--graph ou gitk para visualizar o histórico do repositório.  
* **Aproveite o potencial do stash:** Use o git stash para salvar alterações temporariamente e voltar a elas quando necessário.

### **6\. Recursos para Aprendizado Adicional**

* **Documentação oficial:** [https://git-scm.com/doc](https://git-scm.com/doc)  
* **Tutoriais online:**  
  * Atlassian Git Tutorial: [https://www.atlassian.com/git/tutorials](https://www.atlassian.com/git/tutorials)  
  * GitHub Guides: [https://docs.github.com/en](https://docs.github.com/en)  
* **Cursos gratuitos:**  
  * Projetos Open Source (como exercism.io) oferecem desafios práticos com Git.  
* **Livros de referência:**  
  * "[Pro Git](https://git-scm.com/book/pt-br/v2)" de Scott Chacon e Ben Straub

**Lembre-se:** A prática constante é essencial para dominar o Git. Experimente diferentes comandos e workflows para encontrar o que melhor se adapta ao seu estilo de desenvolvimento.

### **Considerações Finais**

Parabéns por chegar ao final deste guia\! Com os conhecimentos adquiridos, você já possui uma sólida base em Git para iniciar seus projetos. Lembre-se que a prática é fundamental para dominar o Git. Não tenha medo de experimentar diferentes comandos e workflows.

**Algumas dicas finais:**

* **Utilize ferramentas gráficas:** Embora a linha de comando seja poderosa, ferramentas gráficas podem facilitar a visualização do histórico de commits e simplificar algumas operações.  
* **Contribua para projetos open source:** Participar de projetos open source é uma excelente maneira de praticar Git em um ambiente colaborativo.  
* **Explore recursos avançados:** O Git oferece muitas funcionalidades avançadas, como submódulos, hooks e rebasing. Explore esses tópicos quando estiver mais confortável com os comandos básicos.

### **Recursos Adicionais**

Além dos mencionados anteriormente, considere explorar os seguintes recursos:

* **GitLab:** Plataforma de desenvolvimento colaborativo com funcionalidades de Git avançadas.  
* **Bitbucket:** Outra plataforma popular para hospedagem de repositórios Git.  
* **GitKraken:** Ferramenta gráfica popular para Git.  
* **SourceTree:** Outra ferramenta gráfica com boa reputação.

**Lembre-se:** A comunidade Git é bastante ativa e existem muitos fóruns e grupos online onde você pode buscar ajuda e compartilhar conhecimento.

## 

Aliases Git: Acelere seu fluxo de trabalho

**O que são aliases Git?**

Aliases são atalhos personalizados que você cria para comandos Git mais longos ou complexos. Eles permitem digitar menos e agilizar suas tarefas diárias. Imagine ter um comando como git status abreviado para git st\!

**Como criar um alias?**

Para criar um alias, você usa o comando git config. Por exemplo, para criar o alias st para o comando git status, você executaria:

Bash

`git config --global alias.st status`

O parâmetro \--global indica que o alias será válido em todos os seus repositórios. Se você quiser um alias específico para um repositório, omita o \--global.

**Exemplos de aliases úteis:**

* **Status:**  
  * git config \--global alias.st status  
* **Commit:**  
  * git config \--global alias.ci commit  
* **Log:**  
  * git config \--global alias.log "log \--oneline \--graph \--decorate"  
* **Branch:**  
  * git config \--global alias.co checkout  
  * git config \--global alias.br branch  
* **Merge:**  
  * git config \--alias.mg merge  
* **Diff:**  
  * git config \--alias.di diff  
* **Push:**  
  * git config \--alias.pu push  
* **Pull:**  
  * git config \--alias.pl pull

**Personalizando seus aliases:**

Você pode criar aliases mais complexos, combinando vários comandos. Por exemplo, para criar um alias que faz um commit e um push:

Bash

`git config --global alias.cp '!git commit -m "Automated commit" && git push'`

**Onde encontrar seus aliases:**

Os aliases são armazenados em um arquivo de configuração. Para ver seus aliases, execute:

Bash

`git config --list`

**Por que usar aliases?**

* **Aumenta a velocidade:** Digitar menos comandos economiza tempo.  
* **Reduz erros:** Ao usar aliases, você diminui o risco de digitar comandos incorretamente.  
* **Personalização:** Crie aliases que se adaptem ao seu fluxo de trabalho.

**Dicas adicionais:**

* **Seja consistente:** Use uma nomenclatura lógica para seus aliases.  
* **Comece com os comandos mais usados:** Identifique os comandos que você mais utiliza e crie aliases para eles.  
* **Experimente:** Não tenha medo de experimentar e criar seus próprios aliases.

**Conclusão**

Os aliases são uma ferramenta poderosa para aumentar sua produtividade com o Git. Ao criar atalhos personalizados para comandos comuns, você pode se concentrar mais no desenvolvimento do seu código e menos nas tarefas administrativas.

**Gostaria de aprender mais sobre algum outro tópico relacionado ao Git?**

Possíveis tópicos:

* **Branches:** Como criar, mesclar e excluir branches.  
* **Merge vs. Rebase:** Qual a diferença e quando usar cada um?  
* **Git Flow:** Uma estratégia de branching popular.  
* **Git Hooks:** Automatize tarefas com hooks.  
* **Submódulos:** Inclua outros repositórios em seu projeto.

## 

Mais Exemplos de Aliases Git para Acelerar Seu Fluxo de Trabalho

Com base no seu interesse em aliases Git, vamos explorar alguns exemplos adicionais que podem otimizar ainda mais suas interações com o Git:

### **Aliases para Tarefas Comuns**

* **Commitar e pushar:**  
  Bash  
  `git config --global alias.cp '!git commit -m "Automated commit" && git push'`

  Com git cp, você realiza um commit com uma mensagem padrão e em seguida envia as alterações para o repositório remoto.  
* **Criar um novo branch e ir para ele:**  
  Bash  
  `git config --global alias.cob "checkout -b"`

  Para criar um novo branch chamado "feature" e ir para ele, basta digitar git cob feature.  
* **Ver histórico de um arquivo:**  
  Bash  
  `git config --global alias.la "log --follow --name-only --pretty=format:'%h %ad | %s' --date=short arquivo.txt"`

  Com git la arquivo.txt, você visualiza o histórico de commits de um arquivo específico, incluindo data e mensagem do commit.  
* **Stash e pop:**  
  Bash  
  `git config --global alias.st stash`  
  `git config --global alias.po stash pop`

  Simplifica os comandos para salvar e restaurar alterações não commitadas.

### **Aliases Personalizados para Fluxos de Trabalho Específicos**

* **Para desenvolvedores que trabalham com muitas branches:**  
  Bash  
  `git config --global alias.lb "branch -a --contains HEAD"  # Listar branches que contém o commit atual`

* **Para quem precisa frequentemente reverter commits:**  
  Bash  
  `git config --global alias.revert "revert HEAD"`

* **Para quem usa tags extensivamente:**  
  Bash  
  `git config --global alias.tag "tag -a"  # Criar uma tag anotada`

### **Dicas Adicionais**

* **Utilize aliases para tarefas repetitivas:** Se você executa uma sequência de comandos com frequência, crie um alias para ela.  
* **Adapte os aliases ao seu estilo:** Personalize os aliases para que se encaixem na sua forma de trabalhar.  
* **Documente seus aliases:** Crie um arquivo README ou um comentário no seu arquivo de configuração para lembrar a função de cada alias.

**Exemplos de aliases personalizados para diferentes cenários:**

* **Para um desenvolvedor que trabalha em um projeto com muitas integrações:**  
  Bash  
  `git config --global alias.integrate 'merge develop && push origin main'`

* **Para um desenvolvedor que precisa frequentemente criar branches a partir de um ponto específico:**  
  Bash  
  `git config --global alias.newbranch 'checkout -b new-branch <commit-hash>'`

**Lembre-se:** A criatividade é o limite\! Adapte estes exemplos e crie seus próprios aliases para otimizar seu fluxo de trabalho com o Git.

## 

Criando Aliases Git Complexos com Pipes

**O que são pipes?**

Em linhas de comando, pipes (representados pelo caractere |) são utilizados para conectar a saída de um comando à entrada de outro. Isso permite criar sequências de comandos encadeados, onde o resultado de um comando alimenta o próximo.

**Como usar pipes em aliases Git?**

Ao criar aliases Git, você pode utilizar pipes para combinar diferentes comandos e criar fluxos de trabalho mais complexos. Por exemplo, imagine que você queira criar um alias que liste todos os arquivos modificados e não adicionados ao staging area, e em seguida, adicione-os ao staging area. Você poderia criar um alias assim:

Bash

`git config --global alias.staa 'status --short | grep "^M" | cut -c3- | xargs git add'`

**Explicando o alias:**

1. git status \--short: Exibe um status conciso das modificações.  
2. grep "^M": Filtra as linhas que começam com "M", indicando modificações.  
3. cut \-c3-: Extrai a partir do terceiro caractere (o nome do arquivo).  
4. xargs git add: Passa os nomes dos arquivos como argumentos para o comando git add.

**Outro exemplo:**

Suponha que você queira criar um alias para encontrar todos os commits que modificaram um determinado arquivo e mostrar a mensagem de commit:

Bash

`git config --global alias.logfile 'log --grep="^:0:arquivo.txt" --pretty=format:%s'`

**Explicando o alias:**

1. git log: Exibe o histórico de commits.  
2. \--grep="^:0:arquivo.txt": Filtra os commits que modificaram o arquivo "arquivo.txt".  
3. \--pretty=format:%s: Exibe apenas a mensagem de commit.

**Criando aliases personalizados:**

A chave para criar aliases complexos é entender os comandos básicos do Git e como combiná-los usando pipes. Você pode usar outros comandos como grep, sed, awk, find e xargs para criar aliases altamente personalizados.

**Dicas para criar aliases complexos:**

* **Quebre o problema em partes menores:** Divida a tarefa complexa em passos menores e crie um alias para cada passo.  
* **Utilize comandos auxiliares:** Explore comandos como grep, sed e awk para manipular a saída dos comandos Git.  
* **Teste seus aliases:** Antes de usar um alias em um projeto importante, teste-o em um repositório de teste.  
* **Documente seus aliases:** Anote a função de cada alias para que você e outros membros da equipe possam entender como eles funcionam.

**Exemplo de um alias mais complexo:**

Bash

`git config --global alias.fixup 'revert HEAD && commit --amend'`

Este alias reverte o último commit e em seguida permite que você edite a mensagem do commit anterior, efetivamente "consertando" o último commit.

**Conclusão**

Ao dominar o uso de pipes em aliases Git, você pode criar fluxos de trabalho altamente personalizados e eficientes. Experimente diferentes combinações de comandos e descubra como otimizar seu dia a dia com o Git.

## Hooks no Git: Automatize suas tarefas e mantenha a qualidade do código

**O que são hooks no Git?**

Hooks são scripts que são executados automaticamente em determinados pontos do ciclo de vida de um repositório Git. Eles permitem automatizar tarefas, como executar testes, formatar código ou verificar a conformidade com padrões de codificação, antes ou depois de um commit, push, ou outras operações.

**Por que usar hooks?**

* **Automatização:** Elimine tarefas repetitivas e economize tempo.
* **Qualidade do código:** Garanta que o código esteja sempre formatado corretamente e livre de erros comuns.
* **Conformidade:** Force o cumprimento de padrões e convenções de codificação.
* **Integração contínua:** Integre o Git com outras ferramentas, como servidores de build e sistemas de testes.

**Tipos de hooks:**

Existem dois tipos principais de hooks:

* **Client-side hooks:** São executados no computador local do desenvolvedor.
* **Server-side hooks:** São executados em um servidor Git (como o GitHub ou GitLab) e podem ser usados para implementar políticas de acesso, notificações e outras funcionalidades.

**Hooks client-side comuns:**

* **pre-commit:** Executado antes de um commit. Ideal para verificar se o código está formatado corretamente, se os testes passam, etc.
* **post-commit:** Executado após um commit. Pode ser usado para enviar notificações, atualizar documentação ou realizar outras tarefas.
* **pre-push:** Executado antes de um push para o repositório remoto. Pode ser usado para verificar se todos os testes estão passando.
* **post-merge:** Executado após um merge. Pode ser usado para executar scripts de atualização ou limpeza.

**Exemplo de um hook pre-commit:**

```bash
#!/bin/sh

# Verifica se há espaços em branco no final das linhas
git diff --cached --check

# Verifica se os testes passam
npm test
```

**Como criar um hook:**

1. **Localize o diretório de hooks:**
   ```bash
   git rev-parse --git-dir
   ```
   Normalmente, fica em `.git/hooks`.
2. **Crie um arquivo:** Crie um arquivo com o nome do hook desejado (por exemplo, `pre-commit`).
3. **Adicione o script:** Cole o seu script no arquivo.
4. **Tornar o script executável:**
   ```bash
   chmod +x .git/hooks/pre-commit
   ```

**Ferramentas para gerenciar hooks:**

* **Husky:** Simplifica a criação e gerenciamento de hooks.
* **pre-commit:** Permite definir e compartilhar hooks entre projetos.

**Exemplo usando Husky:**

```bash
npx husky install
npx husky add .husky/pre-commit "npm test"
```

**Dicas:**

* **Mantenha seus hooks simples e eficientes:** Hooks complexos podem tornar o processo de desenvolvimento mais lento.
* **Teste seus hooks:** Certifique-se de que seus hooks não causem problemas inesperados.
* **Utilize ferramentas de formatação de código:** Ferramentas como Prettier podem automatizar a formatação do código.
* **Considere usar linters:** Linters como ESLint podem identificar problemas de código antes que eles se tornem um problema maior.

**Conclusão:**

Hooks são uma ferramenta poderosa para automatizar tarefas e garantir a qualidade do código. Ao utilizar hooks de forma eficaz, você pode melhorar significativamente seu fluxo de trabalho e a qualidade do seu projeto.

## Hooks Client-Side para Java: Otimizando seu Fluxo de Trabalho

**Hooks client-side** são scripts que são executados automaticamente em eventos específicos do Git, como antes de um commit ou após um push. Para desenvolvedores Java, eles podem ser uma ferramenta poderosa para automatizar tarefas, garantir a qualidade do código e melhorar a produtividade.

**Sessão 1: pre-commit**

O hook `pre-commit` é executado antes de um commit. É ideal para:

* **Verificar formatação:**
  ```bash
  #!/bin/sh

  # Verifica a formatação do código usando o Checkstyle
  checkstyle -c .checkstyle.xml .
  ```
* **Executar testes unitários:**
  ```bash
  #!/bin/sh

  # Executa os testes JUnit
  ./gradlew test
  ```
* **Verificar licenças:**
  ```bash
  #!/bin/sh

  # Verifica se todos os arquivos possuem a licença correta
  find . -name "*.java" -exec grep -q "Copyright" {} \;
  ```
* **Verificar dependências:**
  ```bash
  #!/bin/sh

  # Verifica se todas as dependências estão listadas no pom.xml
  ./gradlew dependencyCheck
  ```

**Sessão 2: post-commit**

O hook `post-commit` é executado após um commit. É útil para:

* **Criar tags:**
  ```bash
  #!/bin/sh

  # Cria uma tag após um commit para versões específicas
  if [[ $(git rev-parse --abbrev-ref HEAD) == "main" ]]; then
      git tag -a v$(git rev-parse --short HEAD) -m "v$(git rev-parse --short HEAD)"
  fi
  ```
* **Enviar notificações:**
  ```bash
  #!/bin/sh

  # Envia um email para uma lista de destinatários
  /usr/bin/mail -s "Novo commit no projeto" email@example.com < /dev/null
  ```
* **Atualizar documentação:**
  ```bash
  #!/bin/sh

  # Gera a documentação Javadoc após cada commit
  ./gradlew javadoc
  ```

**Sessão 3: pre-push**

O hook `pre-push` é executado antes de um push para o repositório remoto. É útil para:

* **Verificar branch de destino:**
  ```bash
  #!/bin/sh

  # Impede push para branches de produção
  remote=$(git remote -v | grep -oP '^(.*)\s')
  branch=$(git rev-parse --abbrev-ref HEAD)
  if [[ $remote == "origin" && $branch == "main" ]]; then
      echo "Não é permitido push para a branch main"
      exit 1
  fi
  ```
* **Verificar tamanho do commit:**
  ```bash
  #!/bin/sh

  # Limita o tamanho dos commits
  local size=$(git rev-parse --verify HEAD^{tree} --size)
  if [ "$size" -gt 1000000 ]; then
      echo "Commit muito grande. Limite de 1MB."
      exit 1
  fi
  ```

**Sessão 4: post-merge**

O hook `post-merge` é executado após um merge. É útil para:

* **Limpar branches:**
  ```bash
  #!/bin/sh

  # Deleta branches feature após o merge
  local branch=$(git rev-parse --abbrev-ref HEAD)
  if [[ $branch == "main" ]]; then
      git branch -d $(git rev-parse --abbrev-ref HEAD@{1})
  fi
  ```
* **Atualizar dependências:**
  ```bash
  #!/bin/sh

  # Atualiza as dependências após um merge
  ./gradlew dependencyUpdates
  ```

**Considerações importantes:**

* **Personalização:** Adapte os scripts aos seus projetos e necessidades específicas.
* **Testes:** Teste seus hooks em um ambiente seguro antes de usá-los em produção.
* **Ferramentas:** Utilize ferramentas como Husky para simplificar a configuração e gerenciamento de hooks.
* **Linguagem:** Os scripts de hooks podem ser escritos em qualquer linguagem que seu sistema possa executar, mas Bash é uma escolha comum.

**Benefícios dos hooks:**

* **Qualidade do código:** Garante que o código esteja sempre em conformidade com os padrões.
* **Produtividade:** Automatiza tarefas repetitivas.
* **Segurança:** Impede commits e pushes perigosos.
* **Colaboração:** Facilita a colaboração em equipe.

**Conclusão**

Os hooks do Git são uma ferramenta poderosa para melhorar a qualidade do seu código e a eficiência do seu fluxo de trabalho. Ao criar hooks personalizados para suas necessidades, você pode garantir que seu projeto seja sempre bem organizado e livre de erros.



