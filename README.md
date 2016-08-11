# Izie Empresas

## Style Guide

### Typograph
Lato type é a tipografia principal usada

### Font size
```
Headline - <p> 2.4em
Title - <h1> 2em
Subtitle - <h2> 1.6em
Buttons(Bold) - <a> and <button> 1.5em
Details - <small> 1.3em
Body - <p> 1.4em
Line height - 2.5em
```


### Icons
We use [http://fontawesome.io/](Font Awsome)


### Colors
```
Dark blue - #025b91
Navy blue - #3b3e4a
Blue - #008eff
Black - #313131
Dark Gray - #606264
Gray - #dfd9d9
Green - #62be4e
Wine - #a42b56
Dark Orange - e36837
Orange - #fea600
```

### Grid System
O sistema de grid é construída usando uma técnica chamada *Mobile First*, o que significa que todo código é primeiro pensado para a versão enxuta mobile e depois ajustada para as versões de tela maiores.
Nós usamos sempre containers(container), linhas(row) e colunas(col) para representar o sistema de grids.
A a grid é dividida em até 12, que é representada como col-1, col-2, col-3 e etc.


### Header
* Position: static e fixed | Default: static
```
<Header position="fixed" />
```


### Navbar
* posistion: left, right and centered | Default: left
* size: normal, small e large | Default: normal
```
<Navbar position="centered" size="small" /> 
```

### Dropdowns
* size: normal, small e large | Default: normal
```
<Dropdown size="small" />
```

### Alerts
* type: warning, success e error | Default: warning
* icons: Nome do ícone e posição do ícone. ex.: {name: "name-icon", position: (top, right, bottom e left)}
```
<Alert type="success" icon={name: "champion", position: "left"} />
```

### Tables
**Lista de Produtos**
* infos: informações do produto
```
<Table type="productList" infos={id: "CSD01", name: "Produto", type: "produto", price: 20.3, stock: 12} />
```

**Lista de Categorias**
* infos: informações da categoria
```
<Table type="categoryList" infos={id="EFG412", category: "Vinho tinto", out: "10%", productsInCategory: 12, subcategories: [{id="EFG412B", subcategory: "subcategoria 1", out: "2%", productsInCategory: 2}]} />
```

**Kits de Produtos**
* infos: informações dos kits de produtos
```
<Table type="kits" infos={id: "JKSD01", name: "Kit 1", price: 978.99} />
```

**Histórico de Comunicação**
* infos: informações do histórico de comunicação
```
<Table type="comunicationHistory" infos={id="EFG412", title: "título", subtitle: "subtítulo", sendDate: "14:30:00 2016-03-01", status: "ok", users: 100, views: 70, clicks: 10, linkReport: "wwww"} />
```

**Lista de usuários**
* infos: informações da lista de usuários
```
<Table type="userList" infos={id="EFG412", name: "Lista facebook", users: 100} />
```

**Embaixadores**
* infos: informações da lista de usuários
```
<Table type="ambassadors" infos={id="9891231", name: "Maria augusta", avatar: "avatar.jpg" users: 100, status: "ativo"} />
```


### Schedule
* type: month, week e day 
* Infos: Um objeto com todoas as informações: cor, título, visualizações, inscritos, hora, engajamento, cliques
```
<Schedule type="month" infos={color: "blue", title: "título", views: 3000, subscribe: 100, time: "12:03", engagement: 13, clicks: 90} />
```


### Form
* inline: true ou false | Default: false

**Filedset**
* text: String com o texto do fieldset
```
<Filedset text="Fieldset" />
```

**Label**
* text: String com o texto do label
* obs: String com uma observação do campo
```
<Label text="Nome" obs="Preencha seu nome completo" />
```

**Inputs**
* type: text, number, email, password, checkbox, radius, file, tel, date, search, color
* placeholder: Placeholder do input
* icon: Nome do ícone e posição do ícone. ex.: {name: "name-icon", position: (right e left)}
* prefix: normal ou money | Default: normal
* mask: normal, telefone, monetário, cep ou percent| Default: normal
```
<Input type="email" placeholder="Digite aqui seu email" icon={name: "name-icon", position: "right"} >
```

**Checkbox Card**
* format: normal ou card | Default: normal
```
<Input type="checkbox" placeholder="Digite aqui seu email" format="card" >
```

**Textarea**
* placeholder: String com o texto do fieldset
* height: Number
```
<Textarea placeholder="Fieldset" height={10} />
```

**Select**
* placeholder: String com o texto do fieldset
* items: Um array com todos os items ex.: ["item 1", "item 2", "item 3"]
```
<Select placeholder="Fieldset" items={["item 1", "item 2", "item 3"]} />
```

**Image Preview**
* size: normal, small e large | Default: normal
* component: Qual componente ele é ligado
```
<ImagePreview size="large" component="inputImage" />
```

**Estado de validação (Success, Error, Warning)**


### Buttons
Os botoões podem usar as tags *a*, *button* e *input*.
* text: texto do botão
* color
* size: normal, small e large | Default: normal
* type: link, button e submit | Default: button
* filled: true ou false |  Default: true
* state: active e disabled | Default: active
* icons: Nome do ícone e posição do ícone. ex.: {name: "name-icon", position: (top, right, bottom e left)}
* *Estados dos botões: active, hover, focus, visited e disabled.*

```
<Button text="Buscar" color="dark-blue" size="large" type="link" state="disabled" filled={false} icon={name: "search", position: "right"} >
```


### Images and Thumbnails (Figure)
* src: link da imagem
* size: normal, small e large | Default: normal
* type: normal, rounded, circle e thumbnail | Default: normal
```
<Image src="/nome-da-imagem.jpg" size="small" type="circle" />
```


### Cards
**With image**
* type: product e user | Default: product
* Infos: Um objeto com título, subtítulo e preço. {title: "título", subtitle: "subtítulo", price: Number}
Estados: Para escolher e para remover
```
<Card type="product" infos={title: "título", subtitle: "subtítulo", price: 290,00} />
```

**Comunication Cards**
* color
* Infos: Um objeto com todoas as informações: título, visualizações, inscritos, hora, engajamento, cliques. ex.: {title: "título", views: Number, subscribe: Number, time: "12:03", engagement: Number, clicks: Number}
```
<CardComunication color="orange" infos={title: "título", views: 3000, subscribe: 100, time: "12:03", engagement: 13, clicks: 90} />
```


### Pagination
* filled: true ou false |  Default: true
* color
```
<Pagination filled={false} color="green" />
```


### Tags (normal and pills)
* color
* type: normal e pills | Default: normal
```
<Tag color="blue" type="pill" />
```


### Progress Bar and Loading
* color
```
<ProgressBar color="gray" />
<Loading />
```


### Responsive embed
* src: Link do vídeo
```
<Embed src="https://www.youtube.com/watch?v=bAFRlRUPaNQ" />
```


### Lists
* type: normal ou count | Default: normal
* items: objeto com os itens, ícones e posição dos ícones. ex.: {name: "nome", icon: "name-icon", positionIcon: (top, right, bottom e left)}
```
<List type="normal" items={name: "Tarefas", icon: "task", positionIcon: "left"} /> 
```


### Step by step
* color
* type: linear ou dots | Default: linear
* steps: quantidade de passos | Default: 1
```
<Step color="dark-blue" type="dots" steps={10}/>
```


### Modal
* size: normal, small e large | Default: large
* infos: Um objeto com todas as infos
```
<Modal size="normal" infos={title: "Toro loco Tempranilho 2014", price: 200, category: "Vinho tinto", qnty: 20, ... } >
```

### Popover
* direction: top, right, bottom e left
* tag: cor e tipo da tag.: {color: "blue", type: "pill"}
```
<Popover direction="bottom" tag={color: "blue", type: "pill"} />
```


### Tooltip
* direction: top, right, bottom e left
* color
```
<Popover direction="right" color="black" />
```


### Smartphone preview
* background: link com a imagem de fundo
* logo: Imagem do logo
* primary-color: Qualquer cor hexadecimal
* secunday-color: Qualquer cor hexadecimal
```
<Smartphone background="background-image.png" logo="log.png" primary-color="#de34af" secunday-color="#de3466">
```


### Filter
* Component-filtered: Qual componente será filtrado
```
<Filter component-filtered="table" >
```


### Helpers Classes
clearfix
position


