## Lab1: Criar entidades e relacionamentos na plataforma Neo4j Aura

### Modelagem

- Foi utilizada a plataforma: https://arrows.app/ para o desenvolvimento da modelagem.

['lab-01-Modelagem-Streaming_Platform_DIO.png'](lab-01-Modelagem-Streaming_Platform_DIO.png)

### Filmes

```
 Não Fale o Mal
 O Sobrevivente
 O Procurado
 Predador: Terras Selvagens
 Twisters
 Predador: Assassino de Assassinos
 Predador: A Caçada
 Guardiões da Galáxia
 Guardiões da Galáxia Vol. 2
 Guardiões da Galáxia Vol. 3
```

- Atributos: Título, Data do lançamento e duração.
- Fonte: https://www.adorocinema.com

### Demais entidades

```
 Pessoa(diretor)
 Pessoa(ator)
 Pessoa(usuário)
 Genero
```

### Relacionamentos

```
 Filme -> Genero: TEM_GENERO
 Filme -> Diretor: DIRIGIDO_POR
 Ator -> Filme: ATUOU_EM
 Usuário -> Filme: ASSISTIU, atribuindo nota ao filme.
```

### Resultados

['lab-01-neo4j-dio-01.png'](lab-01-neo4j-dio-01.png)

['lab-01-neo4j-dio-02.png'](lab-01-neo4j-dio-02.png)

#### Filrado todos os filmes com relacionamento ASSISTIU exibindo a nota recebida.

Graph view:

['lab-01-neo4j-dio-03.png'](lab-01-neo4j-dio-03.png)

Table view:

['lab-01-neo4j-dio-03.png'](lab-01-neo4j-dio-03.png)

Painel do Neo4j Aura:
['lab-01-neo4j-dio.png'](lab-01-neo4j-dio.png)

Download da view produzida:
['visualisation-lab-01.png'](visualisation-lab-01.png)

### Licença

Este repositório está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
