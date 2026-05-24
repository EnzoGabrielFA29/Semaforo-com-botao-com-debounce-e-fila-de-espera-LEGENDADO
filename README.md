# 🚦 Semáforo Inteligente para Pedestres com ESP32

Projeto desenvolvido utilizando ESP32 e ESP-IDF com o objetivo de simular o funcionamento de um semáforo inteligente para pedestres.

O sistema realiza o controle automático dos LEDs do semáforo e detecta solicitações de travessia através de um botão com debounce por software.

---

Funcionalidades

- Controle de estados do semáforo:
  - Verde
  - Amarelo
  - Vermelho

- Sistema de solicitação de travessia
- Debounce implementado por software
- Contagem de pedidos pendentes
- Controle automatizado utilizando lógica de estados
- Temporização com FreeRTOS
- Simulação compatível com Wokwi

---

Tecnologias Utilizadas

- Linguagem C
- ESP32
- ESP-IDF
- FreeRTOS
- Wokwi

---

Componentes Utilizados

- ESP32
- 3 LEDs
- 1 botão
- Resistores
- Jumpers
- Protoboard

---

Estrutura do Projeto

- `seguir()` → Controla o estado verde
- `atençao()` → Controla o estado amarelo
- `parar()` → Controla o estado vermelho
- `travessia()` → Executa a lógica de travessia
- `botao_pressionado()` → Realiza leitura do botão com debounce

---

Conceitos Aplicados

Durante o desenvolvimento foram utilizados conceitos como:

- GPIO
- Estruturas condicionais
- Loops
- Funções
- Variáveis globais
- Debounce
- Controle de estados
- Automação
- Temporização
- Programação embarcada

---

Funcionamento

1. O semáforo inicia no estado verde.
2. Ao pressionar o botão:
   - O sistema registra um pedido de travessia.
3. Após finalizar o ciclo atual:
   - O sistema libera a travessia.
4. Os LEDs executam a sequência programada.
5. Após o tempo de travessia:
   - O sistema reinicia o ciclo automaticamente.

---

Simulação

O projeto foi desenvolvido e testado utilizando a plataforma Wokwi.

---

Objetivo do Projeto

O objetivo principal foi praticar conceitos de automação, programação embarcada e controle lógico utilizando ESP32.

Além disso, o projeto serviu como base para estudos futuros envolvendo sensores, IoT e sistemas automatizados.

---

Autor

Enzo Gabriel Fernandes de Araújo
Projeto acadêmico desenvolvido no SENAI.
