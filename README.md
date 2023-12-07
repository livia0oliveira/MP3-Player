## Proposta
Projetos de equipes de duplas para entregar até o dia 14/12 (valendo a nota N2)

Projeto 1 (inglês)


Projeto do site: https://fun-javascript-projects.com/course

Neste site você encontrará vários projetos em Javascript com ví­deos explicando como cada projeto foi feito, passo a passo
No entanto, os códigos fontes do projeto podem ser encontrados no github, mais especificamente, na página: https://github.com/chrisdixon161/fun-javascript-projects.com


Após clonar e executar o web app na sua máquina - para garantir que ele está funcionando - proceder com as modificações listadas abaixo.

Para este trabalho, você deverá modificar o projeto nº6 (MP3 Player), conforme itens abaixo.

1) Substituir a imagem do fone de ouvido por uma outra de seu gosto. Crie sua própria, se você souber (usando a tag svg, por exemplo) ou procure uma na internet. Neste caso, busque por "royalty free images", de preferência imagens vetoriais e com fundo transparente.

2) Modificar a cor de fundo do player para a cor de sua preferência

3) Modificar a fonte usada no player para a de sua preferência

4) Modificar as músicas com as suas preferidas. 

5) Exibir na lista de músicas o título apenas, sem a extensão do arquivo.

6) Explique, com suas próprias palavras, o que faz o seguinte trecho de código:

``` bash
const createSongList = () => {
  const list = document.createElement("ol");
  for (let i = 0; i < songs.length; i++) {
    const item = document.createElement("li");
    item.appendChild(document.createTextNode(songs[i].slice(0,-4)));
    list.appendChild(item);
  }
  return list;
};
```

7) Modifique o código para quando vc clicar sobre a barra de progresso, a música avançar para o ponto correspondente

## Resposta - 6

A funçãoo cria o elemento html usando document.createElement("ol"). Entra em um loop "for" que se extende pelo tamanho de sua lista de músicas (songs) e cria um elemento ("li") para cada música. Cada ("li") contém um texto, que é o nome da música sem os últimos 4 caracteres (usando slice(0, -4)). Por fim, cada ("li") é anexado à lista ordenada ("ol").

``` bash
<ol>
    <"li> Never going to give you up.mp3 </li>
</ol>
``` 
