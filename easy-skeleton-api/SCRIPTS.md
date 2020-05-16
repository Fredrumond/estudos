### Scripts

Aqui você encontra informações sobre a utilização de cada script utilizando no workflow do projeto.
``` json
{
	"start": "node src/server.js",
	"dev": "nodemon src/server.js --ignore tests",
	"test": "NODE_ENV=test jest --passWithNoTests",
	"pretest": "NODE_ENV=test sequelize db:migrate",
	"posttest": "NODE_ENV=test sequelize db:migrate:undo:all",
	"test:unit": "npm test -c jest-unit-config.js",
	"test:integration": "npm test -c jest-integration-config.js",
"test:ci": "npm test -- --coverage",
"test:staged": "npm test -- --findRelatedTests"
}
```
| comando | descrição |
|--|--|
| start | Para rodar em produção |
| dev | Para rodar em desenvolvimento |
| test | Realiza todos os testes do sistema |
| pretes | Antes de realizar o teste roda as migrates do banco |
| postest | Apos rodar o teste remove as migrates do banco |
| test:unit | Testa apenas os testes unitarios |
| test:integration | Testa apenas os testes de integração |
| test:ci | Testes de integração contínua |
| test:staged | Testes de arquivos na staged area |



