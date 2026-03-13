# Computação Gráfica com OpenGL

Repositório criado para armazenar exercícios e estudos da disciplina de **Computação Gráfica** do curso de **Sistemas de Informação**.

## Tecnologias Utilizadas

- C++
- OpenGL
- GLUT

---

# Exercícios

## Exercício 1 — Formas Básicas

Este programa cria uma janela gráfica utilizando OpenGL e desenha:

- Um quadrado amarelo  
- Um triângulo verde  
- Duas linhas brancas (horizontal e vertical)

### Conceitos utilizados

- Pipeline gráfico básico
- Renderização de primitivas
- Sistema de coordenadas do OpenGL
- Uso das funções `glBegin()` e `glEnd()`

### Primitivas utilizadas

- `GL_QUADS`
- `GL_TRIANGLES`
- `GL_LINES`

---

## Exercício 2 — Mover um quadrado com o Teclado

**Objetivo:**  
Usar um quadrado e permitir sua movimentação utilizando as teclas **W, A, S, D** sem limitação.

**Dica:**  
Utilizar `GL_TRIANGLE_FAN` e um `for` para gerar os vértices do quadrado.

---

## Exercício 3 — Limitar Movimento dentro da Tela

**Objetivo:**  
Modificar o código para impedir que o objeto saia da área visível da janela.

**Desafio:**  
A área de visualização vai de **-1.0 a 1.0** nos eixos **X** e **Y**.  
Utilizar estruturas `if` para verificar os limites antes de atualizar as posições.

---

## Exercício 4 — Mudar Cor com Teclas Numéricas

**Objetivo:**  
Permitir que o usuário altere a cor do objeto usando as teclas numéricas.

**Teclas:**

- `1` → Vermelho
- `2` → Verde
- `3` → Azul

Criar variáveis de cor:

## Exercício 5 — Movimento com Setas do Teclado

Objetivo:
Controlar o movimento do quadrado utilizando as setas do teclado.

Controles:

Seta para esquerda → move o quadrado para a esquerda

Seta para direita → move o quadrado para a direita

Seta para cima → move o quadrado para cima

Seta para baixo → move o quadrado para baixo

Dica:
Utilize a função glutSpecialFunc() para capturar as teclas especiais do teclado.

Teclas utilizadas:

GLUT_KEY_LEFT

GLUT_KEY_RIGHT

GLUT_KEY_UP

GLUT_KEY_DOWN

Conceitos utilizados:

Manipulação de teclas especiais

Atualização de posição de objetos

Renderização de primitivas com OpenGL

## Exercício 6 — Múltiplos Objetos Independentes

Objetivo:
Adicionar dois quadrados com cores diferentes na tela e permitir que cada um seja movimentado de forma independente.

Controles:

Quadrado 1

W → mover para cima

A → mover para esquerda

S → mover para baixo

D → mover para direita

Quadrado 2

I → mover para cima

J → mover para esquerda

K → mover para baixo

L → mover para direita

Desafio extra:
Criar uma função reutilizável para desenhar os quadrados, evitando repetição de código.

Exemplo de função:

drawSquare(float x, float y, float r, float g, float b)

Essa função recebe:

posição X

posição Y

valores de cor (vermelho, verde e azul)

Conceitos utilizados:

Renderização de múltiplos objetos

Controle independente de objetos

Organização e reutilização de código em funções
