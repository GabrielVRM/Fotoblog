# Fotoblog

## projeto!

![Captura de tela 2024-05-15 185058](https://github.com/GabrielVRM/Fotoblog/assets/95998556/44edf8db-6294-4817-8cf1-2de249b79a56)


### Variaveis de css


### Proporção de IMG
    aspect-ratio: 16/9;
    object-fit: cover;
- aspect-ratio: coloca as imagens no mesmo tamanho e proporção <br>
- object-fit: ajusra a imagen de forma que ela não fique desproporcional, independente do width ou height escolhido


### CSS filter
    filter: hue-rotate(7deg) contrast(101%) saturate(200%);
- mudando satuarçaõ, contrast e rotação da img, normalmente usado com hover! <br>

### CSS transform
    transform: scale(1.1) rotate(-2deg);
- mudando a scale da propriedade, também usado com hover! <br>

### CSS transition
    transition: all 200ms ease-out;
- colocando um tempo para fazer as transições de scale e cores!!

### CSS animation
> propriedade de animação: Keyframes <br/>
> site de animações: animista.net

o minimo para ter uma animação 

- animation-name 
- animation-duration
- keyframes com o nome da animação
  
       .square {
        animation-name: move;
        animation-duration: 1s;
        animation-fill-mode: forwards;
        }
            .square {
            animation-name: move;
            animation-duration: 1s;
            animation-fill-mode: forwards;
        }

        @keyframes move {
          /* from */
          0% {
          }
    
          /* to */
          100% {
        transform: translateX(calc(100vw - 100% - 16px));
          }
                    }

  ### Possibilidades animations:
    - duração: animation-duration
    - direção: animation-direction
    - tempod eexecução: animation-iteration-count: infinite
    - quando irá starta: animation-delay
    - pausar ou iniciar: animation-play-state
 
### Colacando variaveis no keyframes, para manipular um elemento de cada vez com o delay!
  >  HTML <br>
  
                    <figure class="item" style="--delay: 1.4s">
                      <img src="./assets/unsplash_LAY19dUD_ro.png" alt="" />
                      <figcaption class="details">
                        <h2>Organização e grids</h2>
                        <div class="tags">
                          <span>tag</span>
                        </div>
                      </figcaption>
                    </figure>
> css <br>

        .item{
            --delay: .2s;
            animation: appear 1s var(--delay) backwards ;
        }
        @keyframes appear{
        
            0%{
                opacity: 0;
                transform: scale(0.7);
            }
        
        }

  ### Shorthand
      animation: move 1s forwards alternate infinite, blink 100ms infinite;

  
    
  
