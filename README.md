# 1. Animação dos Paragrafos

A Primeira animação foi adicionada aos textos (paragrafos) na linha 57 a 59 do arquivo style.css

```ruby
  animation: paraDireita 1ms ease-in-out forwards;
  animation-timeline: view();
  animation-range: cover 0% cover 30%;
```

- `animation` : Aqui, é definida a animação chamada `paraDireita`, com uma duração de 1 milissegundo, usando uma curva de temporização `ease-in-out`, para suavizar o início e o fim da animação. A propriedade `forwards` indica que, após a animação, os estilos finais devem ser mantidos.

- `animation-timeline: view();` : Esta linha pode estar definindo uma linha do tempo chamada `view()` para a animação. As linhas do tempo podem ser usadas para controlar o momento em que uma animação começa ou termina.

- `animation-range: cover 0% cover 30%;` : Isso pode estar indicando a faixa de aplicação da animação. Parece especificar que a animação deve cobrir a partir de 0% até 30% do tempo total da animação.

## 1.1. Adicionando a Animação

A amimação dos paragrafos foi feita na linha 103 a 112 do arquivo style.css

```ruby
@keyframes paraDireita {
    from {
        opacity: 0;
        translate: -100vw 0;
    }
    to {
        opacity: 1;
        translate: 0 0;
    }
}

```

- `from` : Define os estilos iniciais da animação, neste caso, a opacidade é 0 e o elemento é transladado -100vw horizontalmente.

- `to` : Define os estilos finais da animação, onde a opacidade é 1 e o elemento não tem mais deslocamento horizontal.

# 2. Animação das Imagens

Para animar as imagens foi adicionada a seguinte animação dentro da tag img na lina 73 a 75 do arquivo style.css

```ruby
animation: animacaoParaImagens 1ms ease-in-out both;
animation-timeline: view();
animation-range: entry 25% cover 50%;
```
- `animation` : Aqui, é definida a animação chamada `animacaoParaImagens` , com uma duração de 1 milissegundo e uma curva de temporização `ease-in-out` . O valor `both`  indica que a animação deve aplicar tanto os estilos iniciais quanto os finais.

- `animation-timeline: view();` : Semelhante ao primeiro bloco, isso esta associado a uma linha do tempo `chamada view()` .

- `animation-range: entry 25% cover 50%;` : Isso indica uma faixa de aplicação diferente da primeira animação. Significar que a animação começa no momento de 25% do total e cobre até 50%.

## 2.1. Adicionando a Animação

A amimação das Imagens (img) foi feita na linha 123 a 132 do arquivo style.css

```ruby
@keyframes animacaoParaImagens {
    from {
        opacity: 0;
        clip-path: inset(45% 20% 45% 20%);
    }
    to {
        opacity: 1;
        clip-path: inset(0% 0% 0% 0%);
    }
}
```

Aqui, from e to definem a transição de estilos. No início, a opacidade é 0 e um `clip-path` é aplicado para recortar a imagem. No final, a opacidade é 1 e o `clip-path` é removido.

<hr>

> [!WARNING]
> Lembre-se, a análise detalhada de animações pode depender do contexto específico da aplicação e do HTML associado. Essas interpretações são baseadas nas convenções típicas de animações CSS.

# Contacto 

Em Caso de Dúvidas Entre em Contacto Comigo Através dos Seguintes Canais

<div align='center'>
  <a href="mailto:heliocarlitosantonio@gmail.com" target="_blank"><img src='https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white'/></a>
<a href="https://wa.me/258862867990?text=Ol%C3%A1%20*H%C3%A9lio%20Carlitos*%2C%20eu%20sou%20%5BSeu%20Nome%20Completo%5D%2C%20peguei%20seu%20contacto%20no%20" target="_blank"><img src='https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white'/></a>

</div>
