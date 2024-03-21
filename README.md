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

Caso seja uma preocupação sua, lembre-se de no final da aula remover as chaves geradas na máquina local e também no GitHub, repetindo este procedimento sempre que quiser acessar o GitHub do LabGrad:

```
rm ~/.ssh/id_ed25519
rm ~/.ssh/id_ed25519.pub
```


## Configurando o usuário e o email no git

Use os seguintes comando para conseguir configurar o email e o usuário no git na máquina local

```bash
git config --global user.email "seuemail@email.com"
```

```bash
git config --global user.name "seunome"
```


Para checar se já há algum usuário e email configurado ou chegar se as configurações foram aplicadas, use o comando a seguir

```bash
git config --list
```




## Fazendo commit

A flag _'-a'_ faz o add automaticamente de todos os arquivos *modificados*. Os novos arquivos não são adicionados.


Caso você delete um arquivo no seu diretório, estará untracked a remoção do mesmo. Você pode usar o git rm para colocar em stage a remoção.


## TESTE
