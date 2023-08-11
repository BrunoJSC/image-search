# Aplicativo de Busca de Imagens usando a API da Unsplash

Este repositório contém um aplicativo web simples que permite aos usuários buscar imagens usando a API da Unsplash. O aplicativo obtém imagens com base na consulta de pesquisa do usuário e exibe os resultados em um formato de grade. Os usuários também podem carregar mais imagens clicando no botão "Mostrar Mais".

## Começando

Para usar este aplicativo, siga estas etapas:

1. **Obtenha uma Chave de Acesso à API da Unsplash:**
   Você precisará de uma chave de acesso à API da Unsplash para fazer solicitações à API. Se você ainda não possui uma, pode se inscrever no [Portal do Desenvolvedor da Unsplash](https://unsplash.com/developers) para obter sua chave de API.

2. **Clone o Repositório:**
   Clone este repositório para sua máquina local usando seu método preferido. Você também pode baixar o código-fonte como um arquivo ZIP, se preferir.

3. **Insira Sua Chave de Acesso à API:**
   Abra o arquivo `index.js` e localize a seguinte linha:
   ```javascript
   const accessKey = "aS-LTCdIwU3tkxjW58FI3dC4NxgzrWs9qFKpDiaw03I";
   ```
   Substitua `"aS-LTCdIwU3tkxjW58FI3dC4NxgzrWs9qFKpDiaw03I"` pela sua chave de acesso real da API da Unsplash.

4. **Abra o Arquivo HTML:**
   Abra o arquivo `index.html` em um navegador da web ou hospede-o em um servidor local.

5. **Busque Imagens:**
   Insira uma consulta de pesquisa no campo de entrada e clique no botão "Buscar" ou pressione Enter. O aplicativo exibirá os resultados da pesquisa em um formato de grade.

6. **Carregue Mais Imagens:**
   Se desejar ver mais imagens, basta clicar no botão "Mostrar Mais" na parte inferior dos resultados da pesquisa.

## Como o Código Funciona

O arquivo `index.js` contém o código JavaScript que alimenta o aplicativo. Aqui está uma visão geral de sua funcionalidade:

- O código começa definindo constantes e variáveis para armazenar elementos do documento HTML, chave de acesso à API, dados de entrada e o número da página atual.

- A função `searchImage` é responsável por buscar imagens na API da Unsplash com base na consulta de pesquisa do usuário. Ela constrói a URL da API usando a chave de acesso à API e a consulta de pesquisa. Em seguida, faz uma solicitação de busca e processa a resposta JSON para extrair os dados das imagens.

- Os resultados da pesquisa são exibidos no HTML criando elementos DOM para cada imagem e anexando-os ao container `searchResults`. A função `map` é usada para iterar pelos dados das imagens e gerar os elementos HTML necessários.

- Os ouvintes de eventos são configurados para o evento de envio do formulário de pesquisa e para o clique no botão "Mostrar Mais". Quando o formulário é enviado, a função `searchImage` é chamada para realizar uma nova pesquisa e redefinir o número da página. Clicar no botão "Mostrar Mais" busca imagens adicionais sem redefinir o número da página.

## Contribuições

Contribuições para este projeto são bem-vindas! Sinta-se à vontade para fazer um fork do repositório, fazer alterações e enviar solicitações de pull.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).

---

Boa busca de imagens! Se você encontrar algum problema ou tiver ideias para melhorias, não hesite em abrir uma issue ou contribuir para o projeto.
