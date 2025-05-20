# Inteli-Activity-10

**Explicação:** 

**Explique com suas palavras o papel de cada camada da arquitetura MVC usada neste projeto.**
Como o Model, o Controller e a View interagem entre si?

**Resposta:** O Model ele está responsável pela conexão com a estrutura de banco de dados, interagindo assim com o controller que está responsável por cordenar as informações através de uma api entre o Model e o View, justamente sendo essa interação que o Controller faz para que no View o frontend seja exibido para o cliente e as informações puxadas desde o Model passando pelo Controller sejam entregues.

**Como ocorre o envio e o recebimento de dados no formato JSON neste projeto?**
Cite uma rota que responde em JSON e explique seu funcionamento.

**Resposta:**

Um exemplo de rota que responde em JSON seria:

router.get('/api/exemplo', (req, res) => {
  res.json({
    mensagem: "Rota funcionando!",
    status: "ok",
  });
});

seu funcionando é basicamente criar um endereço que neste caso é do tipo GET ou seja ele é feito para o usuário ler um dado, e responder com um dado tipo JSON que possuíra um objeto de mensagem e um objeto de status.

**Qual a importância de usar HTML básico com formulários e tabelas para organizar e manipular dados no navegador?**
Por que esse tipo de estrutura ainda é útil em projetos back-end com Node.js?

**Resposta:** A importância vem do fato que com essa estrutura é possível criar qualquer tipo de requisição incluindo GET, POST, UPDATE, DELETE, sendo a forma mais simples de fazer com que o View consiga se conectar com a API que está no Controller e assim chegar no Model para ele requisitar os dados. Sendo este o motivo do porque é tão útil o HTML básico com formulários e tabelas para organizar e manipular dados no navegador.
