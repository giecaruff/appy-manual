---
title: Comandos
nav_order: 8
description: "Capitulo sobre comandos do Appy"
---

# Capítulo 7 - Comandos

Diversos outros comandos mais específicos desenvolvidos para o appy são
apresentados na seção **COMMAND**, como por exemplo, diferentes métodos
de cálculos petrofísicos, a calculadora de perfis, entre outros. A
seguir serão detalhados como executar cada um desses comandos.

## 7.1 Batch import LAS file

Com a execução do comando _Batch import LAS file_ é possível importar
diversos arquivos LAS presentes em uma única pasta, para o projeto
carregado.

**Passo 1:** No menu principal, clique no botão **COMMAND**.

**Passo 2:** Clique no botão **RUN COMMAND**. Em seguida, uma nova
janela se inicializará para escolher o comando desejado.

![](data/images/image2.png)
**Passo 3:** No seletor _Select command_, clique no comando _Batch
import LAS file_.

![](data/images/image17.png)
**Passo 4:** No primeiro campo disponível, _LAS file folder path_,
digite o caminho da pasta em que contém os arquivos LAS a serem
importados.

![](data/images/image5.png)
**Passo 5:** Em seguida, no campo _File extension_, digite LAS para a
extensão do arquivo LAS.

![](data/images/image20.png)
**Passo 6:** Caso deseje filtrar arquivos presentes na pasta
selecionada, no campo _Regular Expression_, digite uma expressão regular
correspondente.

**Passo 7:** Clique no botão **RUN** para executar o comando. Após
realizada, o poço referente a cada arquivo LAS importado será adicionado
no banco de dados do projeto e o menu lateral será atualizado.

## 7.2 Calculadora de perfis

A execução do comando _Log Calculator_, permite calcular um novo perfil
a partir de uma equação informada. Os perfis presentes no banco de dados
do projeto carregado podem ser utilizados como parâmetros.

**Passo 1:** No menu principal, clique no botão **COMMAND**.

**Passo 2:** Clique no botão **RUN COMMAND**. Em seguida, uma nova
janela se inicializará para escolher o comando desejado.

**Passo 3:** No seletor _Select command_, selecione o comando _Log
Calculator_.

**Passo 4:** No primeiro campo, _Well name_, digite o nome do poço,
disponível no banco de dados, que deseje utilizar os perfis e também
salvar o perfil criado.

**Passo 5:** Informe o nome do grupo de curvas, no campo _Well log set
name_.

**Passo 6:** Para todos os perfis utilizados na equação, informe os
mnemônicos separados por vírgula, no campo _Well log names_.

**Passo 7:** Em _Equation_, digite a equação que deseja realizar. Para
utilizar os perfis informados anteriormente, basta escrever os
mnemônicos da mesma forma na equação.

**Passo 8:** No campo _Output curve name_, digite o nome do perfil
criado como resultado da execução do comando.

**Passo 9:** Clique no botão **RUN** para executar o comando. Após
finalizado, o novo perfil criado será salvo no banco de dados do grupo
de curvas selecionado no passo 5 e no poço selecionado no passo 4. O
menu lateral também será atualizado.

## 7.3 Cálculos de porosidade

Para calcular o perfil de porosidade existem três diferentes métodos
desenvolvidos na versão atual do appy. Todas as fórmulas das diferentes
metodologias utilizam a biblioteca científica stoneforge, também em
desenvolvimento pelo grupo GIECAR. As etapas para executar os diferentes
métodos são descritas abaixo.

### 7.3.1 Porosidade pelo perfil densidade

**Passo 1:** No menu principal, clique no botão **COMMAND**.

**Passo 2:** Clique no botão **RUN COMMAND**. Em seguida, uma nova
janela se inicializará para escolher o comando desejado.

**Passo 3:** No seletor _Select command_, selecione o comando _Density
Porosity (StoneForge)_.

**Passo 4:** No primeiro campo, _Well name_, digite o nome do poço,
disponível no banco de dados, que deseje utilizar os perfis e também
salvar o perfil criado.

**Passo 5:** Informe o nome do grupo de curvas, no campo _Well log set
name_.

**Passo 6:** Informe o mnemônico referente ao perfil de densidade
(geralmente representado pelo mnemônico RHOB ou RHOZ).

**Passo 7:** Informe o valor da densidade da matriz da rocha.

**Passo 8:** Informe o valor da densidade do fluido presente na rocha.

**Passo 9:** No campo _Output curve name_, digite o nome do perfil
criado como resultado da execução do comando.

**Passo 10:** Clique no botão **RUN** para executar o comando. Após
finalizado, o novo perfil criado será salvo no banco de dados do grupo
de curvas selecionado no passo 5 e no poço selecionado no passo 4. O
menu lateral também será atualizado.

**IMPORTANTE:** Na versão atual do appy ainda não é possível calcular um
perfil por zonas, ou seja, não é possível informar mais de um valor para
o mesmo parâmetro. No caso do cálculo da porosidade será necessário
informar um único valor da densidade da matriz da rocha e do fluído que
representa o poço inteiro.

### 7.3.2 Porosidade pelo perfil neutrão

**Passo 1:** No menu principal, clique no botão **COMMAND**.

**Passo 2:** Clique no botão **RUN COMMAND**. Em seguida, uma nova
janela se inicializará para escolher o comando desejado.

**Passo 3:** No seletor _Select command_, selecione o comando _Neutron
Porosity (StoneForge)_.

**Passo 4:** No primeiro campo, _Well name_, digite o nome do poço,
disponível no banco de dados, que deseje utilizar os perfis e também
salvar o perfil criado.

**Passo 5:** Informe o nome do grupo de curvas, no campo _Well log set
name_.

**Passo 6:** Informe o mnemônico referente ao perfil neutrão (geralmente
representado pelo mnemônico NPHI ou NPOR).

**Passo 7:** Informe o mnemônico referente ao perfil de volume de argila
calculado.

**Passo 8:** Informe o valor do perfil neutrão para os folhelhos.

**Passo 9:** No campo _Output curve name_, digite o nome do perfil
criado como resultado da execução do comando.

**Passo 10:** Clique no botão **RUN** para executar o comando. Após
finalizado, o novo perfil criado será salvo no banco de dados do grupo
de curvas selecionado no passo 5 e no poço selecionado no passo 4. O
menu lateral também será atualizado.

### 7.3.3 Porosidade Gaymard-Poupon

**Passo 1:** No menu principal, clique no botão **COMMAND**.

**Passo 2:** Clique no botão **RUN COMMAND**. Em seguida, uma nova
janela se inicializará para escolher o comando desejado.

**Passo 3:** No seletor _Select command_, selecione o comando _Gaymard
Porosity (StoneForge)_.

**Passo 4:** No primeiro campo, _Well name_, digite o nome do poço,
disponível no banco de dados, que deseje utilizar os perfis e também
salvar o perfil criado.

**Passo 5:** Informe o nome do grupo de curvas, no campo _Well log set
name_.

**Passo 6:** Informe o mnemônico referente ao perfil de densidade
(geralmente representado pelo mnemônico RHOB ou RHOZ).

**Passo 7:** Informe o mnemônico referente ao perfil neutrão (geralmente
representado pelo mnemônico NPHI ou NPOR).

**Passo 8:** No campo _Output curve name_, digite o nome do perfil
criado como resultado da execução do comando.

**Passo 9:** Clique no botão **RUN** para executar o comando. Após
finalizado, o novo perfil criado será salvo no banco de dados do grupo
de curvas selecionado no passo 5 e no poço selecionado no passo 4. O
menu lateral também será atualizado.

## 7.4 Cálculo do volume de argila

Para calcular o perfil que representa o volume de argila existem três
diferentes métodos desenvolvidos na versão atual do appy: método linear,
método larionov, método larionov para rochas terciárias. Todas as
fórmulas das diferentes metodologias utilizam a biblioteca científica
stoneforge, também em desenvolvimento pelo grupo GIECAR. As etapas para
executar os diferentes métodos são descritas abaixo.

**Passo 1:** No menu principal, clique no botão **COMMAND**.

**Passo 2:** Clique no botão **RUN COMMAND**. Em seguida, uma nova
janela se inicializará para escolher o comando desejado.

**Passo 3:** No seletor _Select command_, selecione o comando _Shale
Volume (StoneForge)_.

**Passo 4:** No primeiro campo, _Well name_, digite o nome do poço,
disponível no banco de dados, que deseje utilizar os perfis e também
salvar o perfil criado.

**Passo 5:** Informe o nome do grupo de curvas, no campo _Well log set
name_.

**Passo 6:** Informe o mnemônico referente ao perfil de raios gama
(geralmente representado pelo mnemônico GR).

**Passo 7:** Informe o valor mínimo do perfil de raios gama (GR).

**Passo 8:** Informe o valor máximo do perfil de raios gama (GR).

**Passo 9:** No campo _Method_, informe qual método deseja ser utilizado
para calcular o perfil de volume de argila. Pode ser escolhido apenas um
dentre os três métodos disponíveis: _linear, larionov ou
larionov_terciary_.

**Passo 10:** No campo _Output curve name_, digite o nome do perfil
criado como resultado da execução do comando.

**Passo 11:** Clique no botão **RUN** para executar o comando. Após
finalizado, o novo perfil criado será salvo no banco de dados do grupo
de curvas selecionado no passo 5 e no poço selecionado no passo 4. O
menu lateral também será atualizado.

## 7.5 Cálculo da saturação de água

Para calcular o perfil que representa a saturação de água, existe apenas
um método desenvolvido na versão atual do appy, o método por meio da
equação de Archie. O software utiliza as fórmulas e equações
necessárias, da biblioteca científica _StoneForge,_ também em
desenvolvimento pelo grupo GIECAR. As etapas para executar o comando são
descritas abaixo.

**Passo 1:** No menu principal, clique no botão **COMMAND**.

**Passo 2:** Clique no botão **RUN COMMAND**. Em seguida, uma nova
janela se inicializará para escolher o comando desejado.

**Passo 3:** No seletor _Select command_, selecione o comando _Shale
Volume (StoneForge)_.

**Passo 4:** No primeiro campo, _Well name_, digite o nome do poço,
disponível no banco de dados, que deseje utilizar os perfis e também
salvar o perfil criado.

**Passo 5:** Informe o nome do grupo de curvas, no campo _Well log set
name_.

**Passo 6:** Informe o mnemônico referente ao perfil de resistividade
profunda (geralmente representado pelo mnemônico RT ou ILD).

**Passo 7:** Informe o mnemônico referente ao perfil neutrão (geralmente
representado pelo mnemônico NPHI ou NPOR).

**Passo 8:** Informe o valor da resistividade da água.

**Passo 9:** Informe o fator de tortuosidade (a), da equação de Archie.

**Passo 10:** Informe o expoente de cimentação (m), da equação de
Archie.

**Passo 11:** Informe o expoente de saturação (n), da equação de Archie.

**Passo 12:** No campo _Output curve name_, digite o nome do perfil
criado como resultado da execução do comando.

**Passo 13:** Clique no botão **RUN** para executar o comando. Após
finalizado, o novo perfil criado será salvo no banco de dados do grupo
de curvas selecionado no passo 5 e no poço selecionado no passo 4. O
menu lateral também será atualizado.
