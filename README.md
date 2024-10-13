# DBT-Core
DBT *(Data Build Tool)* é uma ferramenta que irá se comunicar única e exclusivamente com o banco de sua escolha. Para sua intalação correta é necessário escolher qual o [banco que irá trabalhar](https://docs.getdbt.com/docs/supported-data-platforms).

## Inicializando o DBT-Core
Utilizar o comando abaixo e seguir as instruções
```bash
dbt init
```
### Configurando o dbt
    * dbname: northwind
    * host: localhost
    * pass: postgress
    * port: 55432
    * schema: public
    * threads: 1
    * type: postgres
    * user: postgres

Neste repositório o docker-compose está apenas com as imagens do pdAdmin e do banco postgres, por isso é necessário configurar o host como *localhost*, pois a comunicação entre dbt e banco de dados é local-container.

Para verificar se todas as dependências estão instaladas, utilize o comando a seguir na pasta onde foi instalada o 'dbt_project.yml' (este nome é dado na configuração do projeto)
```bash
dbt debug
```
