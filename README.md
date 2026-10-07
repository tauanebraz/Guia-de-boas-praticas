# # 📘 Guia Básico de Git e GitHub: Clonagem e Branches
### 1. Acesse o repositório no GitHub
Primeiro, abra o **GitHub** e acesse a organização ou seu perfil. Em seguida, vá até a lista de **repositórios** e escolha o repositório que deseja clonar.

Dentro do repositório, clique no botão **Code**

### 2. Copie a URL do repositório
Ao clicar em **Code**, será aberta uma janela com algumas opções de conexão.

Selecione **HTTPS** e clique no botão de copiar para copiar a URL do repositório.

Ex.: `https://github.com/usuario/nome-repositorio.git`

📌 **Observação:** Se você já tiver uma chave SSH configurada no GitHub, também pode utilizar a opção **SSH**.

### 3. Abra o VSCode e o terminal
Após copiar a URL do repositório, abra o Visual Studio Code (VSCode).

No VSCode, abra o terminal integrado, utilize o atalho padrão:

**Ctrl + `** 

Para abrir um **novo terminal**, utilize:

**Ctrl + Shift +  `**

📌 **Observação:** Caso você tenha personalizado os atalhos do VSCode, os comandos acima podem ser diferentes. Nesse caso, desconsidere os atalhos informados e utilize o atalho que você configurou para abrir o terminal.

### 4. Clone o repositório
No terminal, utilize o comando abaixo, **substituindo a URL de exemplo pela URL que você copiou do seu repositório:**

      git clone https://github.com/usuario/nome-repositorio.git

Pressione **Enter** e aguarde o Git finalizar o processo.

### 5. Abra o projeto no VSCode
Após finalizar a clonagem, digite:

      code .
      
Pressione **Enter**.

O `.` representa a pasta atual, ou seja, o repositório que acabamos de clonar.

O projeto será aberto **em uma nova janela do VSCode**, já com todos os arquivos do repositório disponíveis.

### 6. Verifique se o repositório está conectado

No terminal, execute:

      git remote -v

Você deverá visualizar algo semelhante a:

origin  `https://github.com/usuario/meu-repositorio.git` (fetch)

origin  `https://github.com/usuario/meu-repositorio.git` (push)

Isso confirma que o repositório local está conectado ao repositório remoto do GitHub.

📌 **Observação:** O endereço exibido deve ser o mesmo do repositório que você acabou de clonar.

### 7. Crie uma nova branch
Caso queira fazer alterações no projeto sem modificar diretamente a `main`, você pode criar uma nova branch para trabalhar de forma independente.

Para verificar em qual branch você está:

                  git branch

A branch atual será indicada pelo `*`.

Para **criar uma nova branch** e mudar automaticamente para ela:

                  git switch -c nome-da-branch

Ao usar `git switch -c`, a nova branch é criada **a partir da branch em que você está no momento** e você muda automaticamente para ela.

**O que significa?**

* `git switch` → usado para mudar de branch.
* `-c` → indica que você quer criar uma nova branch.
                
💡 **Curiosidade:** Também é possível criar uma branch pela interface do VSCode. Basta clicar no nome da branch atual, como `main`, na barra inferior e selecionar **Create New Branch** após isso digite o nome da nova branch e pressione **Enter**. O VSCode criará a branch e mudará automaticamente para ela.




















