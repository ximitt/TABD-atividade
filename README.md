# cqlsh

cqConnected to Test Cluster at 127.0.0.1:9042

[cqlsh 6.1.0 | Cassandra 4.1.6 | CQL spec 3.4.6 | Native protocol v5]

Use HELP for help.

cqlsh> CREATE KEYSPACE tech_women

... WITH replication = {

... 'class': 'SimpleStrategy',

... 'replication_factor': 1

... };

cqlsh>

cqlsh> use tech_women

... ;

cqlsh:tech_women> CREATE TABLE tech_women.professionals_woman (

... id UUID PRIMARY KEY,

... name text,

... birth int,

... country text,

... area text,

... contribuition text

... );

cqlsh:tech_women>

cqlsh:tech_women> INSERT INTO tech_women.professionals_woman (id, name, birth, country, area, contribuition)

... VALUES (uuid(), 'Ada Lovelace', 1815, 'Reino Unido', 'Matemática, Programação', 'Primeira programadora de computadores.');

cqlsh:tech_women>

cqlsh:tech_women> INSERT INTO tech_women.professionals_woman (id, name, birth, country, area, contribuition)

... VALUES (uuid(), 'Grace Hopper', 1906, 'Estados Unidos', 'Ciência da Computação, Linguagens de Programação', 'Criadora do primeiro compilador e da linguagem COBOL.');

cqlsh:tech_women>

cqlsh:tech_women> INSERT INTO tech_women.professionals_woman (id, name, birth, country, area, contribuition)

... VALUES (uuid(), 'Hedy Lamarr', 1914, 'Áustria', 'Inventora, Comunicações sem fio', 'Co-inventora de uma técnica que serviu de base para Wi-Fi e Bluetooth.');

cqlsh:tech_women>

cqlsh:tech_women> INSERT INTO tech_women.professionals_woman (id, name, birth, country, area, contribuition)

... VALUES (uuid(), 'Radia Perlman', 1951, 'Estados Unidos', 'Redes de Computadores', 'Criadora do Spanning Tree Protocol (STP), fundamental para o funcionamento da Internet.');

cqlsh:tech_women>

cqlsh:tech_women> INSERT INTO tech_women.professionals_woman (id, name, birth, country, area, contribuition)

... VALUES (uuid(), 'Katherine Johnson', 1918, 'Estados Unidos', 'Matemática, Ciência da Computação', 'Cálculos cruciais para missões espaciais da NASA.');
