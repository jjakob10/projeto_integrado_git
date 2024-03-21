# Repositório de testes do uso de git para a disciplina de projeto integrado

## Criando uma chave ssh e adicionando ela no github

Para interagir com o github autorizado por meio de uma chave ssh siga o processo a seguir

```bash
ssh-keygen -t ed25519 -C "email@email.com"
```

Acesse a chave criada

```bash
gedit ~/.ssh/ed25519.pub
```

Acesse as configurações do github e adicione a chave gerada

Essa é achave pública. No mesmo diretório é gerada uma chave privada que não deve ser compartilhada


## Configurando o usuário e o email no git

Use os seguintes comando para conseguir configurar o email e o usuário no git na máquina local

```bash
git config --global user.email "seuemail@email.com"
```

```bash
git config --global user.name "seunome"
```






## Fazendo commit

A flag _'-a'_ faz o add automaticamente de todos os arquivos *modificados*. Os novos arquivos não são adicionados.


Caso você delete um arquivo no seu diretório, estará untracked a remoção do mesmo. Você pode usar o git rm para colocar em stage a remoção.
