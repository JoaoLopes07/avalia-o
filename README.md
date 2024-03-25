const express = require('express'); /*Importando o módulo express*/

const avaliacao = express(); /*Definindo a sua variável*/

const PORT = 2000; /*Definindo a sua porta*/

avaliacao.get('/', (req,res) => { /*Criando a página webview*/
    res.send('Hello world'); /*Definindo a mensagem que irá aparecer no web*/
    console.log('Página Atualizada'); /*Mostrando que atualizou a página no terminal*/
});

avaliacao.listen(PORT, () => { /*Inicia a avaliação na porta definida*/
    console.log('O Servidor está sendo executado na porta: ${PORT}'); /*Mostrando que a avaliação foi iniciada na porta escolhida no terminal*/
});
