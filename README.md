# Villa da Serra

Guias do hóspede das locações de temporada, publicados em
<https://villadaserra.github.io/>.

## Estrutura

```
/                  página inicial, lista os imóveis
/golden-sea/       guia da Cobertura Golden Sea, Enseada, Guarujá
```

Para um imóvel novo, crie uma pasta no mesmo formato, por exemplo `/paraty/`,
copie o `index.html` de `golden-sea` para dentro dela, troque as fotos e edite
o conteúdo. Depois acrescente um cartão na página inicial.

## Como editar o conteúdo de um guia

Abra `golden-sea/index.html` e procure por `const GUIA = {`. Todo o texto está
nesse objeto, até a linha `fim do conteúdo editável`. Não é preciso mexer em
mais nada do arquivo.

Texto escrito entre colchetes duplos vira etiqueta amarela de pendência na
página, para você não esquecer de preencher.

## Fotos

Ficam na mesma pasta do guia. Cada foto tem duas versões: `01.jpg` é a grande,
usada ao ampliar, e `01t.jpg` é a miniatura da galeria. A lista e as legendas
estão no `const FOTOS`, logo antes do `const GUIA`. `capa.jpg` é a foto da capa
e também a imagem que aparece na prévia do link.

Para trocar uma foto, suba um arquivo com o mesmo nome por cima.

## Publicação

GitHub Pages serve a branch `main` a partir da raiz. Qualquer commit entra no ar
em cerca de um minuto.
