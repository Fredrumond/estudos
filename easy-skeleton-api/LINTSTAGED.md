### Lint-staged

O pacote pode ser encontrado aqui em [lint-staged](https://www.npmjs.com/package/lint-staged)

É um pacote muito simples de utilizar que facilita bastante o workflow. Permite executar scripts na staged area.

##### Instalação
`npm install lint-staged`
##### Configuração
A configuração pode ser realizada de duas maneiras, adicionando no `package.json` ou criando um arquivo na raiz do projeto chamado `.lintstagedrc.json`

O conteúdo da configuração: 
``` json
{
	"*":  "your-cmd"
}
```

