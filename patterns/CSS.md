# CSS

## Table of Contents

- Indentação
- Sintaxe básica
- Seletores
- Declaracoes
- Prefixos
- Comentários
- Performance
- Media Queries
- Organizacao
- Pré-processadores
- Build
- Dicas

### Indentação

Use soft-tabs com dois espaços:

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn{
		color: #fff;
}
```

### Sintaxe básica:

Use sempre aspas duplas:

```css
/* bom */
.btn {
	background-image: url("textura.jpg");
	font-family: "Helvetica Neue", sans-serif;
}

/* ruim */
.btn {
	background-image: url('textura.jpg');
	font-family: 'Helvetica Neue', sans-serif;
}
```

Inclua um espaço antes de abrir as chaves da regra:

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn{
	color: #fff;
}
```

Fecha as chaves em uma nova linha:

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn {
	color: #fff;}
```

Inclua um espaço depois do : da declaração:

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn {
	color:#fff;
}
```

Sempre use um ; no fim da declaração:

```css
/* bom */
.btn {
	color: #fff;
}

/* ruim */
.btn {
	color: #fff
}
```

Mantenha sempre uma declaracao por linha:

```css
/* bom */
.nav,
.footer,
.btn {
	color: #fff;
}

/* ruim */
.nav, .footer, .btn {
	color: #fff;
}
```

Separe as regras por uma linha em branco:

```css
/* bom */
.btn {
	color: #fff;
}

.nav-item {
	color: #fff;
}

/* ruim */
.btn {
	color: #fff;
}
.nav-item {
	color: #fff;
}
```

Sempre use caixa baixa:

```css
/* bom */
.nav-item {
	color: #fff;
}

/* ruim */
.Nav-item {
	color: #fff;
}
```

Use hifens para separar os nomes:

```css
/* bom */
.nav-item {
	color: #fff;
}

/* ruim */
.nav_item {
	color: #fff;
}
```

Sempre que usar valores hexadecimais usem sempre reduzidos:

```css
/* bom */
.nav-item {
	color: #fff;
}

/* ruim */
.nav-item {
	color: #ffffff;
}
```

Não especifique unidades quando o valor for igual a zero:

```css
/* bom */
.nav-item {
	padding: 0;
}

/* ruim */
.nav-item {
	padding: 0px;
}
```

Não use valores iniciados com zero:

```css
/* bom */
.nav-item {
	transition: color .3s;
}

/* ruim */
.nav-item {
	transition: color 0.3s;
}
```

### Seletores

Evite usar nomes muitos curtos e sempre use nomes relacionados a funcao

### Declaracoes

Declaracao agrupadas pela funcao

- Posicionamento
- Box model
- Tipografia
- Visual

dentro de cada categoria as decalracoes devem estar em ordem alfabetica

### Prefixos

Idente cada propriedades alinhada verticalmente para facilitar a edicao mult linha.

### Performance

Nunca use ID

nunca use seletores genericos (elementos)

Use sempre classes

minificacao

### Media Queries

Mobile first

Mantenhas as media queries o mais proximo possivel da regra que ela altera, nuca os separe em arquivos diferentes

### organizacao

Separar logicamente distintas partes do codigo



### Pre processadores

Ao usar variaveis usem sempre nomes semanticos

Abistraia partes comuns de codico em variaveis etc.

### Comentarios

Tire tempo para descrever componentes, como eles funcionam, suas limitacoes, e o modo como sao construidos, nao deixe outros no time adivinharem o proposito de codigos incomuns ou nao obvios

Coloque comentarios em uma nova linha acima do seu assunto

Evite comentarios no fim da linha

Mantenha o comprimento da linha a um maximo sensivel

use os comentarios para quebrar o codigo em secoes

Dica: configure seu editor para lhe prover com atalhos a geracao do padrao de comentarios acordado.

Exemplos de tipos de comentario:

- Sub secao
- comentario de grupo
- descricao
- comentario basico

### Build

Sempre teste e versione o codigo

### Dicas

Configure seu editor para mostrar os espacos em branco

elimine espacos em branco

use um editor config para ajudar a manter a convencao de organizacao do codigo



```css

```

### Referências
[Idiomatic CSS by necolas](https://github.com/necolas/idiomatic-css/blob/master/translations/pt-BR/README.md)

[Coding style by LFeh](https://github.com/LFeh/coding-style/blob/master/translations/pt-BR/README.md)

[Code guide](http://diegoeis.github.io/code-guide/)
