# Teste back-end Allgoo

Caros candidatos, leiam atentamente as instruções neste README para realizar o teste.

> Antes de começar, prepare seu ambiente.

**Este teste requer:**
- Sua IDE favorita
- Ambiente de desenvolvimento com Python 3.5+ ou Node.js 8+ [explicar o porquê do uso de uma ou de outra linguagem]
- Banco de dados (MongoDB, MySQL) [avaliar a necessidade para uso de banco relacional ou não]

--------

## Tarefas do teste:

**NOTE:** Você está livre em usar o framework que desejar. Apenas, gostaria de uma explicação do porquê da sua escolha.

**Funções necessárias:**
  - O usuário precisa se cadastrar e se logar via Rede Social (Facebook ou Twitter ou Google);
  - O usuário poderá compartilhar uma informação pessoal e ter a possibilidade de marcar se ela é verdadeira ou não;
  - Ao compartilhar irá para um mural que poderá ser visualizado por todos os usuários;
  - Neste post outros podem votar se acreditam ou não na informação;
  - Ter um ranking do usuário de acordo com as assertividades dos usuários classificando entre honesto ou mentiroso;
  - Se mais de 3 usuários acertarem o que a informação é, o usuário que deu a informação perde 1 ponto que será dividido entre os 3 e a cada novo usuário o ponto dobra. Exemplo:

    - 3 pessoas acertam = 1 ponto / 3 usuários
    - 4 pessoas acertam = 2 pontos / 4 usuários
    - 5 pessoas acertam = 4 pontos / 5 usuários
    
  - Quando os usuários erram a informação, o ponto é calculado pela quantidade de usuários que erraram (usando o mesmo critério acima), todos os pontos vão para o usuário que deu a informação e são retirados, dos usuários que erraram, os pontos correspondentes. Exemplo:
    - 4 pessoas erraram, cada uma perde 0.5 ponto = (2 pontos / 4 usuários);
    - O usuário que indicou a informação ganha 4 pontos;
    
  - Cada post tem um tempo de duração de exatamente um dia para ser votado. Quando passa desse tempo, encerram-se as votações;
  - Toda transação deve ter Log e esses Logs poderão ser listados por um login admin;
    
## O que queremos de você nesse teste
- Crie em API e/ou microserviços;
- Documente muito bem seu sistema; (pode usar a ferramenta que achar adequada)
- Use docker;
- Implemente testes;
- Faça o deploy do seu sistema em algum server em cloud; (heroku, etc)

## Instruções adicionais

- Faça um fork do repositório
- Testes não são opcionais
- Depois de terminado, envie-nos o link do repositório, a documentação e o link da aplicação.
- Deixe comentários, caso tenha alguma dúvida.
- Implementações sem um README serão automaticamente rejeitadas.

## Bonus / Atividades Opcionais

- Código limpo
- Conhecimento do fluxo da aplicação
- Conhecimento das melhores práticas.
- Criar um endpoint para healthcheck 
   - para a rota `/healthcheck`
   - proponha quais seriam as informações essenciais em um healthcheck ou se não tem necessidade.
- nginx ou alternativa simples de webserver
