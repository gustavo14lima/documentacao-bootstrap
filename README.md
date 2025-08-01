# Documentação Bootstrap - Iniciação ao Framework

## Introdução

Esta documentação tem como objetivo apresentar os principais conceitos e utilitários do **Bootstrap 5.3.7**, um framework front-end responsivo, baseado em HTML, CSS e JavaScript. A seguir, você encontrará instruções de uso, links CDN para inclusão em projetos e os principais componentes e classes utilitárias.

### Iniciando com Bootstrap

Para utilizar o Bootstrap em seu projeto HTML, adicione os seguintes links no seu código:

```
<!doctype html>
<html lang="pt-br">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Bootstrap Demo</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-LN+7fdVzj6u52u30Kp6M/trliBMCMKTyK833zpbD+pXdCLuTusPj697FH4R/5mcr" crossorigin="anonymous">
  </head>
  <body>
    <h1>Hello, world!</h1>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.7/dist/js/bootstrap.bundle.min.js" integrity="sha384-ndDqU0Gzau9qJ1lfW4pNLlhNTkCfHzAVBReH9diLvGRem5+R9g2FzA8ZGN954O5Q" crossorigin="anonymous"></script>
  </body>
</html>
```

## Color

### Cores disponíveis

​	**primary** - azul (usada para hiperlinks, estilos de foco e estados ativos)

​	**secondary** - cinza (texto mais leve)

​	**tertiary** - cinza mais escuro (texto ainda mais leve)

​	**success** - verde (usado para ações e informações positivas ou bem-sucedidas.)

​	**danger** - vermelho (usada para erros e ações perigosas.)

​	**warning** - amarelo (usada para mensagens de aviso não destrutivas.)

​	**info** - azul claro (usado para conteúdo neutro e informativo.)

​	**light** - branco (tema adicional para cores menos contrastantes.)

​	**dark** - preto (tema adicional para cores contrastantes mais altas.)

### Utilitários de Cor para Texto

- `.text-(cor)`
- `.text-opacity-(0 a 100)`

### Utilitários de Cor de Fundo

- `.bg-(cor)`
- `.bg-opacity-(0 a 100)`

### Outras Aplicações de Cor

- `.border`, `.border-(cor)`
- `.btn`, `.btn-(cor)`

## Breakpoints

### Definição

Pontos de corte responsivos baseados na largura da tela.

### Tabela	

| Dispositivo                               | Largura Comum (em px) | Breakpoint Bootstrap        | Sufixo         | Descrição/Exemplo                                  |
| ----------------------------------------- | --------------------- | --------------------------- | -------------- | -------------------------------------------------- |
| Celular pequeno (modo retrato)            | 320 – 575px           | **Extra small (xs)**        | *(sem sufixo)* | iPhone SE, Galaxy A01 — layout padrão mobile       |
| Celular médio/grande                      | 576 – 767px           | **Small (sm)**              | `sm`           | iPhone 14, Galaxy S23 — telas já um pouco maiores  |
| Tablet (modo retrato)                     | 768 – 991px           | **Medium (md)**             | `md`           | iPad, Galaxy Tab, tablets Android comuns           |
| Tablet (modo paisagem) / Laptops pequenos | 992 – 1199px          | **Large (lg)**              | `lg`           | iPad em paisagem, Chromebooks, notebooks compactos |
| Desktop médio/grande                      | 1200 – 1399px         | **Extra large (xl)**        | `xl`           | PCs padrão, monitores de 1080p, iMac, etc.         |
| Monitor ultra-wide / 4K                   | ≥1400px               | **Extra extra large (xxl)** | `xxl`          | Telas grandes, TVs 4K, monitores gamers            |

### Como utilizar

Use as classes com os sufixos de breakpoint (ex: `col-md-6`, `d-lg-none`, etc.).

## Containers

### Tipos

- **`.container`** -> aplica um padding lateral, centralizando o container
- **`.container-fluid`** -> largura de 100%, ocupa a tela por inteira
- **`.container-{breakpoint}`** -> utiliza os valores dos breakpoints predefinidos

## Grid

### Estrutura

- `.container` > `.row` > `.col`

### Atribuições de Largura

- `.col` (automático)
- `.col-{n}` (fixo de 1 a 12)
- `.col-{breakpoint}-{n}` (responsivo)

### Gutter

- Espaço entre colunas
- `.g-0` a `.g-5`, `.gx-*`, `.gy-*`

### Rows

- `.row-cols-{n}` define o número de colunas por linha
- Responsivo com `.row-cols-md-3`, etc.

## Utilitários de Espaçamento

### Margin (`m`) e Padding (`p`)

| Direção        | Abreviação |
| -------------- | ---------- |
| Todas          | `m` / `p`  |
| Topo           | `t`        |
| Base           | `b`        |
| Esquerda       | `s`        |
| Direita        | `e`        |
| X (horizontal) | `x`        |
| Y (vertical)   | `y`        |

#### Exemplo:

- `.mt-3`: margin-top = espaço 3
- `.px-2`: padding horizontal = espaço 2

### Opacidade

- `.opacity-0`, `.opacity-25`, `.opacity-50`, `.opacity-75`, `.opacity-100`

## Tipografia

### Tamanhos de Título

- `.h1` até `.h6` simulam os títulos HTML `<h1>` até `<h6>`
- `.display-1` até `.display-6` criam títulos maiores e mais leves

### Alinhamento

- `.text-start`, `.text-center`, `.text-end`

### Peso da Fonte

- `.fw-bold`, `.fw-semibold`, `.fw-normal`, `.fw-light`

### Estilo da Fonte

- `.fst-italic`, `.fst-normal`

## Botões

### Classes principais

- `.btn`: classe base
- `.btn-primary`, `.btn-secondary`, `.btn-success`, etc.

### Tamanhos

- `.btn-sm`, `.btn-lg`

### Estados

- `.active`, `.disabled`

#### Exemplo:

```
<button class="btn btn-success">Confirmar</button>
<button class="btn btn-outline-danger">Cancelar</button>
```



