# Livros de TI - API

Este repositório contém um arquivo JSON com informações de livros populares na área de Tecnologia da Informação, especificamente voltados para programadores e cibersegurança. Este arquivo pode ser acessado e consumido externamente para fins de teste e experimentação.

## Estrutura do Arquivo JSON

O arquivo JSON, `livros.json`, contém uma lista com 10 livros, cada um com as seguintes informações:

- **Título**: Nome do livro.
- **Autor**: Autor(es) do livro.
- **Área**: Categoria do livro (ex. Programação, Cibersegurança).
- **Imagem**: URL de uma imagem representativa do livro.
- **Editora**: Empresa que publicou o livro.
- **Ano de Publicação**: Ano em que o livro foi publicado.
- **ISBN**: Número padrão internacional do livro.

## Acesso ao JSON

O arquivo JSON pode ser acessado diretamente via URL e pode ser utilizado em projetos como um recurso de dados em formato de API.

- URL de acesso: `https://github.com/MOliveiraf/livros-ti-api.git`

## Exemplo de Consumo com Fetch API

Abaixo está um exemplo de como você pode usar a Fetch API em JavaScript para acessar e manipular os dados do arquivo JSON:

```javascript
fetch('https://raw.githubusercontent.com/MOliveiraf/livros-ti-api/main/livros.json')
  .then(response => response.json())
  .then(data => {
    console.log("Lista de Livros: ", data);
    // Adicione aqui o código para manipular os dados
  })
  .catch(error => console.error('Erro ao buscar dados:', error));