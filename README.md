# Configurações

## Ambientes
* Após montar os ambientes, selecionar seus respectivos ID´s e realizar a configuração no arquivo *versoes.ini*
Exemplo de configuração
    
```sh
        [atual]
        id=3962
        sqlhost=SERVIDORSQL
        sqlbanco=BANCOSQL
        oraclehost=SERVIDORORAACLE
        oraclebanco=BANCOORACLE
```

Editar as configurações do arquivo credenciais.py com as suas credenciais criada no portal do Totvs Restore 
```sh
    credentials.py
        username = "SeuEmailTotvs"
        password = "SenhaSenhaApi"
```

## Utilização
* Para utilizar o CLI basta inica-lo (sempre como administrador);
* No primeiro passo deve-se digitar a versao cadastrada no arquivo *versoes.ini*
    ```sh
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    . + Escoha a versao do RM a ser aberta
    . + Ex 2209
    . + para versao atual apenas aperte Enter
    . +
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    Versao:
    ```
    
* Apos deve-se escolher qual banco de dados utilizar
    ```sh
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    . + Escoha a versao do RM a ser aberta
    . + 1 SQL
    . + 2 ORACLE
    . +
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    Escolha uma das opcoes acima [1,2]?
    ```
* Deve-se escolher Atualizar o ambiente ou apenas unicar o sistema na versão escolhida;
    ```sh
    .. ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    . + Escoha a versao do RM a ser aberta
    . + 1 Atualizar Ambiente
    . + 2 Apenas subir o Host
    . +
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    Escolha uma das opcoes acima [1,2]?
    ```
    
* Caso deseja atualizar, será questionado se deseja apagar o ambiente anterior
    ```sh
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    . + Deseja apagar os arquivos antes de prosseguir atualizando
    . + 1 Não
    . + 2 Sim
    . +
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    Escolha uma das opcoes acima [1,2]?
    ```