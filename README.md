# Explicando a cena 3D feita no Unity

## Sobre a Cena
<p><b>Cena feita por: Cauã Silva e Carlos Alarcon.<b></p>
<p>A cena se baseia em um carro que deve fugir de uma pedra que está rolando em sua direção, porém não é tão simples, o carro precisa desviar de diversos obstáculos indo para os lados, diminuindo seu tamanho e tomando cuidado para não capotar. No final, o carro irá visualizar uma virada que servirá para ele desviar da pedra, assim sobrevivendo e vendo a pedra passar reto. O jogador irá controlar o carro, suas mecânicas são:</p>
<img src='img/comando.png' />

<hr>

## Desenvolvimento da criação da Cena
<img src='img/cena.png' />
<br><br>
<p>Para a criação da cena, foram utilizados diversos GameObjects. São eles:</p>
<ul>
    <li>Cubes</li>
    <li>Sphere</li>
    <li>Main camera</li>
    <li>Directional Light</li>
    <li>Point Light</li>
    <li>Spot Light</li>
    <li>Paredes "invisíveis"</li>
    <li>Assets</li>
    <li>Objetos feitos no Blender</li>
</ul>
<p>O que mais utilizamos foram os Assets, que foi o principal na formação da nossa cena. Os Assets são as árvores, pedras e montanhas, que são bem espalhadas pela cena; Os templos que foram utilizados como decoração da cena; Os obstáculos de rua; Por fim o nosso personagem que é o carro.</p>
<p>O cubo foi utilizado para fazer os pisos e as laterais da estrada onde se passa a cena.</p>
<p>A sphere foi utilizada para fazer a pedra que irá perseguir o carro e para decorações.</p>
<p>O point light foi utilizado para ser um ponto de luz no túnel que foi feito pelo blender.</p>
<p>Foram criados dois spot lights que são os faróis do carro.</p>
<p>Por fim as paredes "invisíveis" foram criadas para que o jogador(carro) não saia da parte principal da cena.</p>

<hr>

### Materiais e textura
<img src='img/materiais.png' />
<p>Os materias foram usados para adicionar texturas aos nossos objetos, nele podemos adicionar imagens de textura ou cores, na nossa cena adicionamos ambos. Aqui estão alguns exemplos de objetos com os materiais:</p>
<br>
<img src='img/exemplomaterial.png' />
<p>Além deles, todos os Assets adicionados já vem com seus materiais a parte.</p>

<hr>

### Box Collider, Sphere Collider e RigidBody
<h4>Exemplo:</h4>
<img src='img/exemplo.png' />
<img src='img/exemplo2.png' />
<br><br>
<p>O box collider foi adicionado nos pisos, no carro(personagem), nos obstáculos e nas laterais e paredes "invisíveis". Ele foi adicionado com a função de fazer com que os objetos não se atravessem, como esse será um jogo onde o carro deverá desviar dos obstáculos enquanto é perseguido por uma pedra, o box collider é essencial. Como mostra a imagem, o box collider é uma caixa de colisão em volta do objeto. Já o sphere collider, como diz o nome, serve para objetos redondos e é uma esfera em volta do objeto, e foi adicionada em todas as sphere adicionadas na cena, mas a principal é a pedra que persegue o carro.</p> 

<p>O RigidBody serve para adicionar os conceitos de física à determinado objeto. Ele foi adicionado ao carro(personagem) e aos obstáculos fazendo assim com que consigam colidir e que fiquem parecidos com a realidade. O único elemento alterado no RigidBody foi o Mass que é a massa do objeto, colocamos uma massa baixa para o carro e uma massa alta para os obstáculos, fazendo com que o carro bata nele e pare.</p>

<hr>

### Scripts
