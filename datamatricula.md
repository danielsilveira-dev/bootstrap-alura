
# data-attributes

O atributo "data-" existe para que possamos adicionar informações customizadas/dinâmicas no DOM, sem utilizar classes nem IDs. Como os sites e aplicações web estão cada vez mais interativos, aumenta também a necessidade de adicionarmos informações específicas no DOM, que não conseguimos cobrir somente com as classes e IDs. Por exemplo, exibir na tela um registro de uma aluna de um banco de dados de alunos de uma escola:

```html
<p id="43oi344y4546y23" class="p-aluna" data-matricula="342543">Nome Aluna</p>
```

No exemplo acima, o atributo `id` está trazendo um valor de ID da entrada da informação no banco de dados (informação única para cada entrada), o atributo `class` está cuidando dos estilos e utilizamos o atributo `data-matricula` para adicionar no DOM uma informação extra que podemos usar como referência (no caso, o número de matrícula).