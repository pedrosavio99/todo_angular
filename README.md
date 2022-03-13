## Sobre o Autor
<img   style="border-radius: 50%"  align="left" width="190" height="190" margin-right="150px"  src="https://lh3.googleusercontent.com/pw/AM-JKLUq-TgjEzhoVY_CtieDZgnZNOoIGyAubOEKisc2FKt7HMCSVv4DGHZjixw4Z2_yomTtgUKr0kxFUyUdmOuTyJnQfhgzXEyOVk6JoajO58wYDtWcrDF-EPRjaE1hj2EsZtM-OYgQsDjHGjdny1yGetxeWw=s250-no?authuser=0"> Oi, meu nome é Pedro Savio, faço engenharia de computação no IFPB, sou desenvolvedor Fullstack e esse é o meu linkedin,  [ir para meu linkedin](https://www.linkedin.com/in/pedro-s-04a300129/).

<br/><br/><br/><br/><br/>


# Todo em Angular Framework

<img    align="left" width="220"  margin-right="150px"  src="https://lh3.googleusercontent.com/pw/AM-JKLW0MQA6HZ-FJj2SxpQe-z_eWORpkz8sEPXQua_LWKzoqlRoAbHbV10G-MmTtXu5HsGCHuZnctkn6aygMFVk837kU_FIpGa-UabULw7xZAIIaipCmDKpmaph7D2ii9oU5R5-QKE_juZVtJLrlB0uBoBlGg=w373-h658-no?authuser=0">
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
<br/>

    ng new angular-todo
    ng serve --open

criar o component todos

    ng g c components/Todos

# Anotações ...
angular é um framework

conceito de spa(Single page applicatiosn deve ser tipo o react)


instalação do angular:

	npm install -g @angular/cli

criar um novo projeto 

	ng new my-first-project

rodar o projeto:
	ng serve --open

add angular material a seu projeto 

	ng add @angular/material

colar isso n aap.module.ts

import { MatSliderModule } from '@angular/material/slider'; ######ISSO DAQUI

@NgModule ({
  imports: [
    MatSliderModule, ##########e isso so
  ]
})
class AppModule {}


========================================
conceitos
componentes igual o react

templates : é o html do component

metadatas: faz o processamento das classes

data binding: assosia dados ao html

services: é onde implmentamos a logica ara ser injetado em classes e componentes n faça a logica no porprio componente

router: responsavel pela navegação 

directives: modifica elementos do dom

============================================

criar um backend local

json-server

npm init
npm i json-server
npm start

paasos, de um cd em backend e faça:

	npm init -y

depos entre no package.json e adicione o script de start

	"start": "json-server --watch db.json --port 3001"

agr intale json server:

	npm i json-server

agr iniciams o servidor local

	npm start


=============== inicar o projeto front

iniciar o projeto angular 
	ng new angular-marketplace

diga sim para criar as rotas e use a estilização padrao class

entendeno o projeto inicial:

src: pasta que contem os componentes da aplicação

app: arquivos ja criado no projeto para estilizar, gerenciar rotas e fazer testes

iniciar a aplicação:
	npm start


============================================================
utilizando o Angular material 
	ng add @angular/material

	CRIAR O HEADER, FOOTER e nav component
	criar  ahome view

em app.modules tem que adicionar os modulos de cada elemento que vc vai usar do material angular

desenvolver a aplicação em app.component.html

==================== crinado um componente ( header )

	ng g c components/templates/header   #aqui vc coloca onde ele vai ficar e o nome dele

mano ai ele cria esse compnente e vc chama ele no app.component.html como uma tag javascript

dai então vc desenvolve ele

==================== crinado um componente ( footer )

	ng g c components/templates/footer


========== importar modulo para o navbar em app.module.ts ja importei tambem o list

==================== crinado um componente ( nav )

	ng g c components/templates/nav
==================== crinado um componente ( card )
	
	ng g c views/home

==================== crinado um componente ( Modelo para  alista de filmes )

	em view cra uma pasta list-filmes e  crie  arquivo film.model.ts

	apos isso vamos criar o primeiro service ou logica de nossa aplkicação

	ng g s views/checkout/checkout

	depois vc desenvolve a logica de chamar os filmes da api

==================== crinado um componente ( Modelo para o cartão do filme )

	ng g c components/templates/card-film

	ng g c views/list-films