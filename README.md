# Eletronics-PowerSupply
O projeto solicitado na disciplina de [SSC0180] – Eletrônica para Computação ministrada pelo professor Eduardo do Valle Simões, da USP envolve a criação de uma fonte de tensão retificadora ajustável. A fonte deve ser capaz de fornecer uma tensão ajustável entre 3V e 12V, com uma corrente mínima de 100mA. 

| Alunos | N°USP |
|----------|----------|
| Felipe Eduardo Dias Tavares | 13713184 |
| Letícia Pinheiro Ferreira | 12683381 |

# Objetivo
Projetar uma fonte de tensão retificadora, ajustável entre 3V e 12V, com capacidade de 100mA.

## &#128161; Componentes utilizados:

* Transformador:

É um componente que muda a tensão elétrica em um circuito. Ele pode aumentar ou diminuir o valor da tensão, dependendo das necessidades do circuito.

* Ponte de diodo:

É um dispositivo usado para converter corrente alternada em corrente contínua. Ele retifica a corrente, permitindo que o circuito seja alimentado em ambas as direções da corrente alternada.

* Capacitor:

É um componente que armazena cargas elétricas. Ele é usado para acumular energia elétrica e liberá-la quando necessário.

* Diodo de Zener:

É um tipo especial de diodo que é usado para regular a tensão em um circuito. Ele mantém a tensão constante em um valor específico, mesmo quando ocorrem variações.

* Resistores:

São componentes usados para controlar o fluxo de corrente elétrica em um circuito. Eles limitam ou ajustam a quantidade de corrente que flui em um determinado caminho.

* Potenciômetro:

É um componente de resistência variável. Ele permite ajustar a voltagem ou a corrente em um circuito, permitindo controlar o fluxo de eletricidade.

* Transistor:

É um componente eletrônico que pode atuar como um interruptor controlado por um sinal elétrico ou amplificar um sinal elétrico. Ele desempenha um papel importante em circuitos eletrônicos, permitindo controlar o fluxo de corrente de acordo com as necessidades do circuito.


# Diagrama da Fonte
![Diagrama da fonte no software Falstad](imagens/Circuito_falstad.png.png)

[Link para o circuito no Falstad](https://www.falstad.com/circuit/circuitjs.html?cct=$+1+0.000005+2.803162489452614+47+5+43%0Av+0+144+0+336+0+1+60+179.6+0+0+0.5%0Ad+112+240+176+176+2+default%0Ad+112+240+176+304+2+default%0Ad+176+304+240+240+2+default%0Ad+176+176+240+240+2+default%0Aw+176+144+176+176+0%0AT+0+144+128+336+0+4+0.1534+-0.034093874954851625+-5.551115123125783e-17+0.999%0Aw+176+304+176+336+0%0Aw+96+240+96+368+0%0Ar+352+240+352+304+0+5600%0Aw+96+240+112+240+0%0Aw+128+144+176+144+0%0Aw+128+336+176+336+0%0Aw+240+240+256+240+0%0Ac+256+240+256+368+0+0.00032999999999999994+26.214973186872953%0Aw+256+368+96+368+0%0A34+z-voltage+0+1.7143528192810002e-7+0+2+12.9%0Az+352+368+352+304+2+z-voltage%0At+480+304+512+304+0+1+-13.461629439350384+0.7145025795592481+100%0Aw+528+240+528+288+0%0Ar+528+320+528+368+0+120%0Aw+496+368+528+368+0%0Aw+496+368+480+368+0%0Aw+256+240+352+240+0%0Aw+256+368+352+368+0%0Aw+352+304+384+304+0%0A174+416+272+448+304+1+10000+0.005+Resistance%0Aw+384+304+384+272+0%0Aw+384+272+384+256+0%0Aw+384+256+416+256+0%0Aw+416+256+416+272+0%0Ar+416+368+416+304+0+5600%0Aw+352+368+416+368+0%0Aw+352+240+448+240+0%0Aw+464+304+480+304+0%0Aw+448+240+528+240+0%0Aw+480+368+416+368+0%0Aw+512+320+528+320+0%0Aw+528+288+512+288+0%0Aw+448+288+464+288+0%0Aw+464+288+464+304+0%0Ao+0+64+0+4099+320+1.6+0+2+0+3+Entrada%0Ao+22+64+0+4099+40+0.2+1+2+22+3+Ap%C3%B3s%5Cso%5Cscapacitor%0Ao+16+64+0+4099+25.696552892723453+0.0027079732569890466+2+2+16+3+Zener%0Ao+18+64+0+4099+40+0.2+3+2+18+3+Coletor%0Ao+33+64+0+4099+20+0.0015625+4+2+33+3+Base%0Ao+19+64+0+4099+20+0.2+5+2+19+3+Sa%C3%ADda%0A)

## :heavy_dollar_sign: Preço dos componentes:


| Quantidade | Componente          | Valor   |
|------------|---------------------|---------|
| 1         | Transformador       | R$63,99 |
| 1          | Ponte de Diodos     | R$6,67  |
| 1          | Capacitor           | R$1,10  |
| 1          | LED                 | R$0,70  |
| 1          | Diodo Zener         | R$0,19  |
| 2          | Potenciômetro       | R$13,58 |
| 1          | Resistor 680        | R$0,38  |
| 1          | Resistor 1k         | R$0,18  |
| 1          | Resistor 3k9        | R$0,38  |
| 2          | Jumper macho x macho| R$13,58 |
| Total      |                     |R$127,81 |


# Projeto Esquemático do PCB no Software Eagle
![Esquema do Eagle](imagens/imagem-eagle-pcb.png "imagem-eagle-pcb.png")
# Projeto Esquemático do circuito no Eagle
![Esquema do Eagle](imagens/imagem-eagle-esquematico.png "imagem-eagle-esquematico.png")



### Capacitor 


$$Ripple = \frac{Vs}{2 \cdot f \cdot C \cdot Req}$$


Onde:

- $Vs$ é a tensão de saída
- $f$ é a frequência
- $C$ é a capacitância
- $Req$ é a resistência de carga

Vamos substituir os valores fornecidos na fórmula:


$$Ripple = \frac{23.506 V}{2 \cdot 120 Hz \cdot 680 \cdot 10^{-6} F \cdot 224.43 \Omega}$$


Agora, vamos calcular isso:

Primeiro, calcule o valor do denominador: 


$$2 \cdot f \cdot C \cdot Req = 2 \cdot 120 Hz \cdot 680 \cdot 10^{-6} F \cdot 224.43 \Omega = 36.5$$


Em seguida, divida a tensão de saída pelo valor calculado: 


$$Ripple = \frac{23.506 V}{36.5} = 0.644 V$$


Portanto, o ripple na saída da fonte de alimentação é de aproximadamente $$0.644 Volts.$$

Porcentagem:
$$\text{Porcentagem do Ripple} = \left(\frac{\text{Ripple}}{Vs}\right) \cdot 100$$

$$\text{Porcentagem do Ripple} = \left(\frac{0.644 V}{23.506 V}\right) \cdot 100 = 2.73 \text{\\%}$$
