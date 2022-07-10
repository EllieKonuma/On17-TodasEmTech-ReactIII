# On17 - ReactJS | Aula 03
![image](https://i.gifer.com/Aro9.gif)

## Recebam minhas boas vindas!

✅ Chamada

✅ Acordos

✅ Apresentação das monitoras

<br>
<br>

______

## Revisão 

| `Conteúdos da aula 01 e 02`                     |  |
| --------------------------- | ------------------ |
| O que é e quem usa react?            
| Preparando o ambiente e "Olá, Mundo!"
| Componentes e JSX
| Props e State
| Eventos (onClick e onChange), listas e chaves
| Introdução aos hooks (useState e useEffect)

<br>
<br>


---

# 🚀 Vambora pra o conteúdo da aula 3?

> ⚠️ Após essa aula você estará preparada para consolidar o entendimento sobre ReactJS.  O objetivo específico da aula é facilitar a criação de um projeto guiado do zero ao deploy.



| `Conteúdos da aula:`                     |  |
| --------------------------- | ------------------ |
| Introdução ao Roadmap React + Próximos passos
| Rotas - React Router       
| Projeto guiado do zero ao deploy

<br>
<br>

# 💜 Roadmap de ReactJS

`Acesse aqui` : [trilha ReactJS](https://miro.com/app/board/uXjVOfD6Q_0=/?invite_link_id=954992108760) 

# 😎 Rotas - React Router

Lembra que com react estamos construindo SPA(single page application)? O que significa dizer que na real a gente só construiu uma única página. E quando a gente precisa criar um menu e algumas páginas diferentes. Precisamos usar uma biblioteca que nos ajude com isso, a construir rotas no react.

Para que no fim das contas, quando clicarmos no menu ou alterarmos na URL a gente consiga visualizar o conteúdo correto. Vamos aprender a usar a biblioteca react-router-dom.

1) Vamos instalar com o npm 

```
npm install react-router-dom@6
```

2) Vamos criar o arquivo que irá gerenciar nossos endereços

```
import {  
  BrowserRouter,
  Routes,
  Route
} from 'react-router-dom';

import Home from '../Pages/Home'
import Sobre from '../Pages/Sobre'
import Portfolio from '../Pages/Portfolio'
import Contato from '../Pages/Contato'

function ApplicationRoutes(){
  return(
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Home />} />
        <Route path="expenses" element={<Sobre />} />
        <Route path="invoices" element={<Portfolio />} />
         <Route path="invoices" element={<Contato />} />
      </Routes>
  </BrowserRouter>
  )
}
export default ApplicationRoutes
```

3) Vamos criar o menu

```
import { Link } from 'react-router-dom'

const Menu = () =>{
  return(
    <ul className="menu">
      <li>
        <Link className="link" to="/">Home</Link>
      </li>
      <li>
        <Link  className="link" to="/sobre">Sobre</Link>
      </li>
      <li>
        <Link  className="link" to="/portfolio">Portfólio</Link>
      </li>
      <li>
        <Link className="link" to="/contato">Contato</Link>
      </li>
    </ul>
  )

}

export default Menu
```

4) Podemos usar o menu nas páginas

5) No app em vez de chamar cada página, iremos usar as Rotas

```
import ApplicationRoutes from './ApplicationRoutes'

function App() {
  return (
    <div>      
      <ApplicationRoutes/>    
    </div>   
  )
}

export default App;
```


`Acesse a documentação oficial`: [React Router](https://reactrouter.com/docs/en/v6)  



# ❤️ Projeto guiado

Passo a passo

[ ]Criar organização das pastas

[ ] Criar rotas

[ ] Criar Menu

[ ] Criar Header

[ ] Criar páginas

  - [ ] Projetos usando axios
  - [ ] Comentários usando localStorage

**Para Quinta**
[ ] Subir no netlify e incluir a configuração de redirects - Quinta-feira

**Para Casa**
[ ] Criar e incluir footer

[ ] Criar e inclir páginas 

  - [ ] Sobre
  - [ ] Diário da reprograma
  - [ ] Contato

### `Tecnologias`

| Ferramenta | Descrição |
| --- | --- |
| `vite` | Gerador de projeto front-end |
| `ReactJS` | Biblioteca javascript|
| `npm` | Gerenciador de pacotes|
| `axios` | Para consumo de API|
| `react-router-dom` | Criador de rotas|
| `netlify` | Hospedagem|
| `react-icons` | Icones grátis|
| `css` | Folhas de estilos|
| `Google fonts` | Fonte|
| `undraw` | Banco de ilustrações grátis|
| 
  
### `Arquitetura`

```
 📁 projeto-guiado
   |- 📁 src
   |     |- 📁 assets
   |     |- 📁 components
   |       |- 📁 Footer
   |       |- 📁 Header
   |       |- 📁 Menu
   |     |- 📁 pages
   |       |- 📁 Sobre
   |       |- 📁 Comentarios
   |       |- 📁 Projetos
   |       |- 📁 Diario
   |       |- 📁 Contato
   |     |- 📁 routes
   |- 📁 node_modules
   |- 📄 app.jsx
   |- 📄 main.jsx
   |- 📄 .gitignore
   |- 📄 package.json  
   |- 📄 package-lock.json
```
---

### `Entregavel da semana` 
- Utilize o mesmo projeto criado em sala de aula para incluir as páginas de `sobre`, `diário da reprograma` e `contato`.

- Lembre-se de incluir essas páginas no menu e na rota também
 

`- Eu fiz o meu, vem aqui entender melhor e se inspirar`: [Meu portfólio da reprograma](https://react-project-3.netlify.app/) 

> Passo a passo:
1) Crie um projeto react com vite
2) Apague as informações default
3) Crie componentes para cada seção (Serão 5 conforme acima)
4) Import no App.jsx os componentes criados para montar o seu portfólio, perceba os erros/warnings que o terminal/console mostra, resolva e faça todos os componentes renderizar na tela 
5) Suba esse projeto no github, atualize o read me contando tudo o que você aprendeu e usou nesta segunda aula. E suba no classroom.
6) Tente fazer em tempo hábil pra aproveitar a aula de quinta e as monitorias pra tirar dúvidas.
7) Arraseee! E qualquer coisa, me chama!

---

_Foi incrível compartilhar essa jornada com vocês! Qualquer dúvida ou sugestão, chama no contatinho!_

### Vamos nos conectar!

- [youtube](https://www.youtube.com/queroserdev)
- [instagram](https://www.instagram.com/simara_conceicao)
- [linkedin](https://www.linkedin.com/in/simaraconceicao/)
- [github](https://github.com/simaraconceicao)
- [spotify](https://open.spotify.com/show/59vCz4TY6tPHXW26qJknh3)
- [quero ser dev](https://queroserdev.com)

<br>
Feito com 💜 por Simara Conceição