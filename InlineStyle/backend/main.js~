var express = require('express');
var app = express();

var contatos = [{nome: "Joao", telefone: "98766789"},
		{nome: "Pedro", telefone: "99879999"},
		{nome: "Mateus", telefone: "99998888"}];

app.get('/contatos', function(req, res){
	res.json(contatos);
});

app.all('*', function(req, res, next) {
  res.header('Access-Control-Allow-Origin', '*');
  res.header('Access-Control-Allow-Methods', 'GET');
  res.header('Access-Control-Allow-Headers', 'Content-Type');
  next();
});

app.listen(process.env.PORT || 3412);
