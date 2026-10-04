<!--!!!! Use CTRL + SHIFT + V para visualizar este documento
no VS CODE -->

# Guia para o projeto do site de Tintas Automotivas

Este documendo estabelece as regras para boa conduta na construção do nosso site utilizando o tríade web HTML, CSS, JS e em conjunto com as linguagens PHP e SQL para manutenção do banco de dados.

## Organização

TODO O CONTEÚDO ESCRITO EM CSS DEVE SEGUIR A MESMA CRONOLOGIA DO CÓDIGO HTML. A HIERARQUIA PRECISA EXISTIR DE FORMA LINEAR.

Exemplo:

html
```html
<tag1>
    <tag2></tag2>
</tag1>
```

css
```css
tag1 {
}
tag2 {
}

```

## Comentários

Os comentários serão um dos principais meios de notas para os desenvolvedores que também usarão o código. podem ser temporários ou não. Os comentários não devem incluir features/recursos pois estes devem ser postos no nosso Kanban 

## Arquitetura Baseada em Módulos

O projeto possui uma estrutura modular onde cada funcionalidade é isolada em um componente próprio no site. cada módulo deve ser organizado com sua própria pasta e seus próprios arquivos.

Cada página deverá conter pasta pai, arquivo html, uma pasta com o seu nome ou identificando seu usuário para que você organize livremente seus projetos nela seguindo a seguinte organização:

    📂 pasta-pai
    ├── 📄 index.html
    |
    ├── 📂 pessoa01
    |   ├── 📄 modulo.js
    |   ├── 📄 estilo-modulo.css
    |   └── 📂 Imagens
    |       |
    |       ├── logo.svg 🖼️
    |       └── imagem1.jpg 🖼️
    |
    ├── 📂 pessoa02
    └── 📂 pessoa03

## Navegação em Caminhos Relativos

A navegação dos arquivos deverá seguir a Navegação por Caminho Relativo como '.' para pasta atual e '..' para navegar em pastas-pai. Serve para evitar conflitos ao manipular o site offline e permitindo que a rotina dos devs sejam híbridas independentes de servidores.

## Padrão de Nomenclatura Único

A padronização visual do código e dos arquivos do projeto segue estritamente o formato dash-case e sem nenhum caractere latino nem acentuação para evitar conflitos.

Todas as pastas, arquivos de linguagem e variáveis criados para os módulos devem utilizar letras minúsculas separadas por hífens. Isso não inclui arquivos de imagens ou ordenados pelo nome.

exemplo:
```
    estilo-header.css

    funcao-teste()

    --cor-fundo-transparente: #ffffff;
```

## Processo de Revisão de Código

A qualidade do sistema depende do alinhamento coletivo e nenhum código pode ser integrado diretamente à versão final sem passar por uma avaliação detalhada. Sempre que um módulo ou funcionalidade for concluído, será realizada uma análise afim de resolver bugs e diagnosticar problemas, conflitos e inconsistências que podem poluir o código.

## FTP (Somente para quem souber gerenciar FTP via linha de comando e afins)

Solicitar o acesso à senha, domínio, nome de usuário e porta para fazer upload de arquivos ou atualizar webpage.