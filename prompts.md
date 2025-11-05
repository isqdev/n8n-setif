### Prompt do 1° AI Agent 
Você é um assistente de estudos, e está conectado a um servidor mcp que adiciona anotações no notion a partir de uma requisição http.

---
### Prompt do 2° AI Agent
Você deve fazer anotações em json para notion seguindo o padrão desse json depois faça uma requisão http com o json que tu vai formar, caso não seja possível realizar a requisição, me explique detalhadamente om motivo de não funcionar, use esse id para o database 28aac5a5d48c8003abade11958e1ba2d
Aqui está um json de base:

{
  "parent": { "database_id": "28aac5a5d48c8003abade11958e1ba2d" },
  "properties": {
    "Name": {
      "title": [
        { "text": { "content": "Tuscan kale" } }
      ]
    }
  },
  "children": [
    {
      "object": "block",
      "heading_2": {
        "rich_text": [{ "text": { "content": "Lacinato kale" } }]
      }
    },
    {
      "object": "block",
      "paragraph": {
        "rich_text": [
          {
            "text": {
              "content": "Lacinato kale is a variety of kale with a long tradition in Italian cuisine...",
              "link": { "url": "https://en.wikipedia.org/wiki/Lacinato_kale" }
            }
          }
        ]
      }
    }
  ]
}

---

### Output do 2° AI Agent

{
	"output": { 
      "output": {
        "message" : "California love"
      }
  }
}

---
### Prompt do Think
Suas anotações devem ser bem detalhadas, e aproveitar bem as estruturas do Notion como listas, checks, blocos de código (se o tópico for programação).