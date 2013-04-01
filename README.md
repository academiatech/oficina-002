# [Academia Tech](http://academiatech.com.br) - Oficina 002
===========

Web Semântica na Prática: **Criando seu Primeiro Modelo Semântico**.

[Rômulo Jales](http://github.com/romulojales) e [Victor Pantoja](http://github.com/victorpantoja)

## Descrição

Se você teve oportunidade de assistir o debate sobre web semântica e ficou querendo mais, essa é a oportunidade! Se você ainda não assistiu, confira [aqui](http://academiatech.com.br/agenda/web-semantica-os-desafios-por-tras-da-nova-web).

## Resumo

O objetivo final desta oficina é apresentar de forma prática os conceitos de web semântica através da criação de uma ontologia que descreve Fórmula 1.

Faremos uma rápida apresentação sobre web semântica, sobre o banco de grafos Virtuoso, SPARQL e demais tecnologias relacionadas

Os desenvolvedores criarão a ontologia baseada no nosso input (domínio e dicionário de dados). A idéia e criarmos os TTLs para cada entidade e carregarmos esses TTLs no Virtuoso utilizando o simple-db-migrate.

Os TTLs serão criados aos poucos, com nosso auxílio. Os desenvolvedores irão criar as queries para inserir dados iniciais na ontologia.

A seguir, faremos consultados SPARQL no grafo que criamos no Virtuoso e explicaremos, na prática, os paradigmas dessa abordagem de programação.

Esperamos com essa oficina que os desenvolvedores saiam com vontade de utilizar semântica em suas apliações

A oficina terá 2 horas de duração:

#### Abertura (15 minutos):

- Apresentação do tema da oficina

#### Demonstração da solução (10 minutos)

- exibir a ontologia final

#### Mão na massa (70 minutos)

- Introdução ao console do Virtuoso

#### Demonstração final (5 minutos)

- exibir a ontologia criada durante o curso

#### Considerações finais (20 minutos)

## Pré-requisitos

Não teremos instruções específicas para Windows. Utilizaremos Mac OSX ou Linux. Preparar o ambiente local com:

* Instalar o gawk, dependência do Virtuoso

```bash
wget http://ftp.gnu.org/gnu/gawk/gawk-4.0.2.tar.gz
tar -xzvf gawk-4.0.2.tar.gz
cd gawk-4.0.2.tar.gz

./configure
make
make install
```

* Instalar o [Virtuoso](http://sourceforge.net/projects/virtuoso/?source=dlp)

```bash
./configure
make
make install
```

Para iniciar o virtuoso:
```bash
/usr/local/virtuoso-opensource/bin/virtuoso-t -f -c /usr/local/virtuoso-opensource/var/lib/virtuoso/db/virtuoso.ini

Usuário dba / dba
```

* Ter o python 2.7, ou superior, com o [pip](https://pypi.python.org/pypi/pip) instalado
* Executar no terminal:

```bash
mkdir -p ~/academiatech && cd ~/academiatech

git clone git@github.com:academiatech/oficina-002.git
cd oficina-002

pip install virtualenvwrapper
mkvirtualenv academiatech
pip install simple-virtuoso-migrate

```
