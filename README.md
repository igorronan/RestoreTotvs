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

Caso deseje visualizar os logs de informações na propria tela do CLI, basta adicionar o trecho abaixo no arquivo de versoes.ini 
```sh
    versoes.ini
        [log]
        info=true
```

## Utilização
* Para tornar mais intuitivo a atulização trouxe a versão grafica para escolha dos ambientes;
* Para utilizar o CLI basta inica-lo (sempre como administrador);
* Para a virada de versão, deve-se obrigatoriamente realizar o cadastro da nova versão no Restore da Totvs (passo Ambientes)
