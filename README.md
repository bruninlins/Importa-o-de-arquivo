<h1 align="center">Script para importar um arquivo CSV para MySQL</h1>

<br>

Este é um script em Python que importa dados de um arquivo CSV para uma tabela MySQL. Ele cria a tabela automaticamente (caso não exista) e insere os dados do arquivo.

<br>

## Requisitos

- Python 3.x
- Biblioteca `pymysql`
- Servidor MySQL em execução
- Um arquivo CSV delimitado por `;`

## Instalação

1. Instale a biblioteca `pymysql`, caso ainda não tenha:
   ```sh
   pip install pymysql
   ```

2. Configure o banco de dados no MySQL:
   - Certifique-se de que o banco de dados especificado existe.
   - Atualize as credenciais no dicionário `db_config` dentro do script.

## Uso

1. Certifique-se de que o arquivo CSV está no mesmo diretório do script.
2. Rode o programa.

## Funcionamento

- O script abre o arquivo CSV e obtém os cabeçalhos.
- Cria uma tabela no MySQL com colunas baseadas nos cabeçalhos do CSV (caso ainda não exista).
- Lê e insere os dados na tabela, normalizando os valores.
- Fecha a conexão com o banco de dados ao final.

## Observações

- Certifique-se de que o banco de dados MySQL está em execução e acessível.
- O script não trata erros relacionados ao formato do CSV, então os dados devem estar bem estruturados.
- Para evitar problemas de segurança, **não armazene credenciais de banco de dados diretamente no código-fonte em produção**.


## Imagem do script funcionando:


![Captura de tela 2025-04-02 191602](https://github.com/user-attachments/assets/df8593a9-008d-4c10-a62c-a60a6be000c2)
