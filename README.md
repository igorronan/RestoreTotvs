# Configurações


## Totvs Restore
* Utilizar o restore disponibilizado pela totvs;
    link para documentação:  https://tdn.totvs.com/pages/releaseview.action?pageId=607585039
    Obrigatorio que a pasta do restore esteja dentro da mesma pasta do atualizador com o nome "restore"

## Ambientes
* Após montar os ambientes no site do restore (https://totvsrestore.z15.web.core.windows.net/#/), selecionar seus respectivos ID´s e realizar a configuração no arquivo *versoes.ini*
Exemplo de configuração
    
```sh
        [atual]
        id=ID
        sqlhost=SERVIDORSQL
        sqlbanco=BANCOSQL
        oraclehost=SERVIDORORAACLE
        oraclebanco=BANCOORACLE
```

Editar as configurações do arquivo versoes.ini com as suas credenciais criada no portal do Totvs Restore 
```sh
    versoes.ini
        username=SeuEmailTotvs
        password=SenhaSenhaApi
```


Definir qual portal será aberto por padrao ao terminar de carregar o ambiente (caso não houver um padrao será o Pontuario Eletronico) 
```sh
    versoes.ini
        [portal]
        default=portalpaciente
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

* Depois deve-se escolher Atualizar o ambiente ou apenas iniciar o sistema na versão escolhida;
    ```sh
    .. ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    . + Escoha a versao do RM a ser aberta
    . + 1 Atualizar Ambiente
    . + 2 Apenas subir o Host
    . +
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    Escolha uma das opcoes acima [1,2]?
    ```


* Por ultimo caso desejar pode-se excluir todo o ambiente antes de subir novamente os novos arquivos;
    ```sh
    .. ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    . + Deseja apagar os arquivos antes de prosseguir atualizando
    . + 1 Não
    . + 2 Sim
    . +
    . ++++++++++++++++++++++++++++++++++++++++++++++++++++++
    Escolha uma das opcoes acima [1,2]?
    ```
