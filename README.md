# Boostrap

## Instalando Bootstrap  

Obs: Nesta aula, foi utilizado o Bootstrap versão 4.3

## Links da documentação do Bootstrap usados na aula: 
[Introdução](https://getbootstrap.com/docs/4.3/getting-started/introduction/) | 
[Navbar](https://getbootstrap.com/docs/4.3/components/navbar/) | 
[Flex](https://getbootstrap.com/docs/4.3/utilities/flex/) | 
[Position: fixed-top](https://getbootstrap.com/docs/4.3/utilities/position/#fixed-top)

Clique em `Docs`.

Vá até **CSS** e copie o link conforme abaixo:  

```html
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
```

Vá até  **Separate** e copie as duas linhas disponíveis pra colar no final do `body`
```html
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
```

## Adicionando uma Navbar

Na barra de pesquisa da documentação do **Bootstrap**, procurei por "Navbar" e procurei uma utilizada na aula:  
[Navbar](https://getbootstrap.com/docs/4.3/components/navbar/)  

```html
<nav class="navbar navbar-expand-lg navbar-light bg-light fixed-top">
  <a class="navbar-brand" href="#">fruta & fruto</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup">
    <div class="navbar-nav">
      <a class="nav-item nav-link active" href="#">início <span class="sr-only">(current)</span></a>
      <a class="nav-item nav-link" href="#">receitas</a>
      <a class="nav-item nav-link" href="#">quem somos</a>
      <a class="nav-item nav-link" href="#">contato</a>
    </div>
  </div>
</nav>
```
### Foram feitas algumas alterações:  
 - Incluído a classe `fixed-top` para fixar o navbar no topo da página ao dar scrol.
 - Inclusão da classe `justify-content-end` no elemento pai do elemento de classe `navbar-nav` para alinhamento do menu à direita.  
 - Retirada a classe `disabled` e os atributos ` tabindex="-1" aria-disabled="true"` do link do menu de navegação.  

## Adicionando carrossel e resolvendo alguns bugs
 - Adicionado classe `imagem-carrossel` nas duas imagens do carousel;