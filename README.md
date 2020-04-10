#### Observações gerais

* Como a API não está implementada, vocês podem escolher como querem receber os dados necessários para construir sua tela. Por exempo: se você recebeu a tela "Meus looks", mas a rota que retorna os looks não está implementada, crie uma variável que contém os dados tais como você gostaria de recebê-los da API. Veja o exemplo do que poderia ser um objeto com dados de entrada:

``` js
const input = [{
    _id: "id_do_look_1",
    name: "nome do look 1",
    description: "descrição do look 1",
    clothe_torso: {
        // Informações da roupa do tronco
    },
    clothe_leg: {
        // Informações da roupa das pernas
    },
    clothe_feet: {
        // Informações do calçado
    }
},
{
    _id: "id_do_look_2",
    name: "nome do look 2",
    description: "descrição do look 2",
    clothe_torso: {
        // Informações da roupa do tronco
    },
    clothe_leg: {
        // Informações da roupa das pernas
    },
    clothe_feet: {
        // Informações do calçado
    }
}
// ...
]
```

* Se você tiver dúvidas ou quiser exemplos de como os dados da API estão estruturados, você pode consultar os arquivos modelo (`*.model.js`) no repositório da API. No caso da tela de "Meus looks", seria interessante saber como os looks e as roupas estão estruturados, para isso você poderia consultar os arquivos `look.routes.js` e `garment.model.js`.