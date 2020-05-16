### Husky

O pacote pode ser encontrado aqui em: [husky](https://www.npmjs.com/package/husky)

É um pacote muito simples de utilizar que facilita bastante o workflow.

##### Instalação
`npm install husky --save-dev`
##### Configuração
A configuração pode ser realizada de duas maneiras, adicionando no `package.json` ou criando um arquivo na raiz do projeto chamado `.huskyrc.json`

O conteúdo da configuração: 
```json
{
	"hooks": {
		"pre-commit": "npm test",
		"pre-push": "npm test"
	}
}
