# Projeto Flask com Monaco Editor

## Estrutura do Projeto

Este projeto utiliza Flask para servir uma aplicação web com o Monaco Editor integrado. A estrutura do projeto é organizada da seguinte forma:

- **`app.py`**: Arquivo principal que configura e inicia o servidor Flask.
- **`templates/`**: Pasta que contém arquivos HTML que são processados pelo Flask para gerar o conteúdo dinâmico da aplicação.
- **`static/`**: Pasta que armazena arquivos estáticos, como CSS, JavaScript e imagens, que são servidos diretamente ao cliente.

## Configuração do Flask

1. **Pasta `templates/`**: Armazena os arquivos HTML. O Flask processa esses arquivos para gerar o conteúdo dinâmico que é enviado ao cliente.

2. **Pasta `static/`**: Contém arquivos estáticos, como folhas de estilo (CSS), scripts JavaScript e imagens. Esses arquivos são servidos diretamente pelo Flask e não são processados.

3. **Uso de `url_for`**: No arquivo HTML, utilize a função `url_for` do Flask para referenciar os arquivos estáticos. Isso garante que os caminhos para os arquivos sejam resolvidos corretamente.

## Benefícios da Estrutura

- **Manutenção Facilitada**: A separação entre templates e arquivos estáticos ajuda a manter o projeto organizado e facilita a manutenção do código.
- **Desempenho**: Arquivos estáticos são servidos diretamente e rapidamente, enquanto templates são processados para gerar conteúdo dinâmico.
- **Funcionalidade**: A configuração permite que os arquivos HTML sejam renderizados corretamente com dados dinâmicos e que os recursos estáticos sejam carregados conforme necessário.

## Como Executar

1. Certifique-se de que todas as dependências estão instaladas.
2. Execute o arquivo `app.py` para iniciar o servidor Flask.
3. Acesse a aplicação web através do navegador em `http://localhost:5000`.

## Observações

- Certifique-se de que o `index.html` esteja na pasta `templates/` e que os recursos estáticos estejam na pasta `static/`.
- Utilize o `url_for` para referenciar recursos estáticos no HTML para garantir o carregamento correto dos arquivos.

