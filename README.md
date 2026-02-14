# 3D Cube Loader

Um componente de carregamento tridimensional elegante e moderno, construído puramente com **HTML5** e **CSS3**. O projeto utiliza manipulação de espaço 3D para criar um cubo giratório com efeitos de iluminação e sombra.

## 🧱 Estrutura do Projeto

O loader é composto por uma arquitetura que simula geometria espacial:

* **`.cube-loader`**: O container principal que define o contexto 3D (`preserve-3d`) e gerencia a animação de rotação contínua.
* **`.cube-wrapper`**: Envolve as faces laterais do cubo.
* **`.cube-span`**: Representa as 4 faces laterais. Utiliza variáveis CSS (`--i`) para calcular a rotação individual de cada face em 90 graus.
* **`.cube-top`**: A face superior do cubo, que também contém um pseudo-elemento `::before` configurado para projetar a sombra brilhante no "chão".

## 🛠 Detalhes Técnicos

### Transformações 3D
O projeto faz uso intensivo de propriedades avançadas do CSS:
* **`transform-style: preserve-3d`**: Permite que os elementos filhos sejam posicionados no eixo Z.
* **`rotateX` / `rotateY`**: Define o ângulo de visão e a animação de giro.
* **`translateZ`**: Desloca as faces a partir do centro para formar o volume do cubo.

### Estilização
* **Gradientes Dinâmicos**: As faces utilizam `linear-gradient` com cores HSL para simular profundidade e reflexos metálicos/neon.
* **Efeito de Brilho (Glow)**: A sombra inferior utiliza `filter: blur()` e múltiplos `box-shadow` para criar uma iluminação difusa que acompanha o movimento do objeto.

## 🚀 Como Utilizar

1.  Copie a estrutura HTML para o seu arquivo principal.
2.  Adicione o CSS ao seu arquivo de estilos.
3.  Para ajustar o tamanho, altere os valores de `width` e `height` na classe `.cube-loader` e ajuste o `translateZ` para metade do novo tamanho.

---
<img width="113" height="131" alt="Image" src="https://github.com/user-attachments/assets/7a754951-da74-4b7f-aa99-cc603c4c8fcb" />
