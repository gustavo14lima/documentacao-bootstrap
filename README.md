 # Color

### Cores disponíveis

​	**primary** - azul (usada para hiperlinks, estilos de foco e estados ativos)

​	**secondary **- cinza (texto mais leve)

​	**tertiary** - cinza mais escuro (texto ainda mais leve)

​	**success** - verde (usado para ações e informações positivas ou bem-sucedidas.)

​	**danger** - vermelho (usada para erros e ações perigosas.)

​	**warning** - amarelo (usada para mensagens de aviso não destrutivas.)

​	**info** - azul claro (usado para conteúdo neutro e informativo.)

​	**light** - branco (tema adicional para cores menos contrastantes.)

​	**dark** - preto (tema adicional para cores contrastantes mais altas.)

### Utilitários de Cor para Texto

​	utilizar a classes **.text-(cor disponivel)**

​	pode-se controlar a opacidade de um texto utilizando a classe **.text-opacity-(valor para a opacidade, utilizando valores de 0 até 100)**

### Utilitários de Cor de Fundo

​	para trocar a cor de fundo, utilize a classe **.bg-(cor disponivel)**

​	é possivel utilizar opacidade na cor de fundo também, utilizando a classe **.bg-opacity-(valor de 0 até 100)**

### Outras Aplicações de Cor

​	pode-se estilizar a cor de uma borda, utilizando a classe 

​		**.border** -> cria uma borda

​		**.border-(cor disponivel)** -> cor para a borda

​	seguindo a mesma linha de raciocínio:

​		**.btn** -> estilizar para se parecer com um botão

​		**.btn-(cor disponivel)** -> cor para o botão



# Breakpoints 

### Definição de Breakpoints

​	São pontos de corte em larguras de tela que definem quando estilos/responsividade mudam. Eles aplicam estilos básicos para todas as necessidades, cobrindo a maioria dos tipos de dispositivos.

​	Existem 6 tamanhos predefinidos:

| Dispositivo                               | Largura Comum (em px) | Breakpoint Bootstrap        | Sufixo         | Descrição/Exemplo                                  |
| ----------------------------------------- | --------------------- | --------------------------- | -------------- | -------------------------------------------------- |
| Celular pequeno (modo retrato)            | 320 – 575px           | **Extra small (xs)**        | *(sem sufixo)* | iPhone SE, Galaxy A01 — layout padrão mobile       |
| Celular médio/grande                      | 576 – 767px           | **Small (sm)**              | `sm`           | iPhone 14, Galaxy S23 — telas já um pouco maiores  |
| Tablet (modo retrato)                     | 768 – 991px           | **Medium (md)**             | `md`           | iPad, Galaxy Tab, tablets Android comuns           |
| Tablet (modo paisagem) / Laptops pequenos | 992 – 1199px          | **Large (lg)**              | `lg`           | iPad em paisagem, Chromebooks, notebooks compactos |
| Desktop médio/grande                      | 1200 – 1399px         | **Extra large (xl)**        | `xl`           | PCs padrão, monitores de 1080p, iMac, etc.         |
| Monitor ultra-wide / 4K                   | ≥1400px               | **Extra extra large (xxl)** | `xxl`          | Telas grandes, TVs 4K, monitores gamers            |

### Como utilizar os Breakpoints?

​	Para utilizar os breakpoints, primeiro, utilize a resolução mais alta, ou seja, a `xxl` que seria para monitores com mais de 1400px, com isso, você vai escrevendo com as demais resoluções!

### Grid e composição

​	O grid pode ser especificado com os valores dos breakpoints predefinidos. Onde, utilizando a classe `col` junto com ums dos breakpoints.

#### 	Exemplo:

​		`.col-md`

​		Aqui, a coluna está sendo especificada com o tamanho `medium`

# Containers

### Tipos de Containers

​	No bootstrap, possui três tipos principais de Containers:

​		**`.container`** -> aplica um padding lateral, centralizando o container

​		**`.container-fluid`** -> largura de 100%, ocupa a tela por inteira

​		**`.container-{breakpoint}`** -> utiliza os valores dos breakpoints predefinidos

# Grid

### Estrutura báscio do Grid	

​	A estrutura básica do Grid segue um padrão composto por três elementos principais:

​		**1.** Container

​		**2.** Row

​		**3.** Column

### Atribuições de Largura

​	Como visto anteriormente, o Grid pode, mais especificamente as colunas, podem utilizar os breakpoints.

​	Mas você também pode definir o tamanho da coluna automaticamente, seguindo um número de 1 até 12, onde 12 ocupa a linha inteira e 1 ocupa 1/12 da linha.

​	Caso apenas especifique **`col`**, o tamanho da coluna será ajustado automaticamente.

### Gutter	

​	Por padrão, cada coluna tem padding horizontal de 0.75 rem, você pode alterar isso utilizando um arquivo CSS interno, assim, podendo alterar o padding e outras propriedades.

### Rows

​	Você pode especificar quantas colunas poderá ter em cada linha, utilizando a propriedade **`row-cols-n`** você especifica a quantidade **n** de colunas que terá em cada linha.

​	Você pode utilizar também os breakpoints, tanto para quantas colunas terá na linha, quanto na linha normal.
