# Painel_Didatico
<img width="1376" height="768" alt="Gemini_Generated_Image_cwpclwcwpclwcwpc" src="https://github.com/user-attachments/assets/4042428b-7999-4757-a5fa-63affebad6c9" />



<h1 align="center"> Entrega - 04</h1>

##

<p align="center">
  <a href="#requisito">Requisitos </a> 
  |
  <a href="#objetivo">Objetivo da Sprint </a>
  |
  <a href="#desenvolvimento">Desenvolvimento </a>
  |
  <a href="#cronograma">Cronograma </a>
  |
  <a href="#conclusao">Conclusão </a>
  
</p>

##

**Início: 06/05  - Fim: 12/06**

**Status da Sprint: Concluído ✅**
<br>
<br>
<br>

<span id="requisito">
  
 ## 📜Requisitos
Desenvolver um painel didático de automação industrial para demonstrar a partida direta e a reversão do sentido de rotação de um motor trifásico, utilizando o CLP Siemens LOGO! como elemento central de controle. O sistema integra circuitos de potência e comando, programação em Ladder, contatores, dispositivos de proteção e sinalização visual e sonora, permitindo demonstrar os princípios de funcionamento e segurança aplicados à automação industrial.

<span id="objetivo">
  
## 📌Objetivo da Sprint
O objetivo desta fase é realizar a validação da solução.<br>

<span id="desenvolvimento">
  
## 📚Desenvolvimento


### Introdução<br>
O desenvolvimento de sistemas de automação industrial permite aplicar conhecimentos de eletricidade, comandos elétricos e programação na construção de soluções para o controle de máquinas e equipamentos. Nesse contexto, o projeto do painel didático de partida direta com reversão tem como objetivo demonstrar o acionamento de um motor trifásico nos sentidos horário e anti-horário, utilizando o CLP Siemens LOGO! como elemento central de controle.
Para isso, o painel integra componentes como contatores, disjuntores, fonte de alimentação de 24 VCC, botoeiras, dispositivos de sinalização e um motor trifásico. A programação é desenvolvida em linguagem Ladder, permitindo controlar os comandos de acionamento, parada e reversão, considerando os intertravamentos elétricos e lógicos e os recursos de proteção do sistema. A integração desses elementos proporciona uma aplicação prática dos conceitos de automação industrial e comandos elétricos.<br>

### Processo<br>
A seguir, são descritos os principais componentes utilizados no desenvolvimento do painel didático de partida direta com reversão via CLP.<br>

• CLP Siemens LOGO!<br>
É o controlador responsável pelo processamento dos comandos e pela execução da lógica de funcionamento do sistema. Por meio da programação em linguagem Ladder, controla as saídas responsáveis pelo acionamento dos contatores e pela sinalização das condições de operação.<br>

• Contatores KM1 e KM2<br>
São os dispositivos responsáveis pelo acionamento do motor trifásico. O contator KM1 realiza a ligação para o funcionamento em um sentido de rotação, enquanto o KM2 realiza a reversão por meio da troca de duas fases da alimentação do motor. O sistema utiliza intertravamentos para evitar o acionamento simultâneo dos contatores.<br>

• Disjuntor de Proteção do Motor<br>
É o componente destinado à proteção do circuito do motor. Além de proteger o sistema, seu contato auxiliar pode fornecer ao CLP uma indicação relacionada à atuação da proteção, permitindo o tratamento dessa condição na lógica de controle.<br>

• Fonte de Alimentação de 24 VCC<br>
É responsável por converter a alimentação de entrada de 220 VCA em 24 VCC, fornecendo energia ao CLP e aos componentes do circuito de comando que utilizam essa tensão.<br>

• Botoeiras de Comando<br>
São utilizadas para enviar os comandos de operação ao sistema. Permitem solicitar a partida em cada sentido de rotação e realizar a parada do motor. Esses sinais são processados pelo CLP conforme a lógica programada.<br>

• Botão de Emergência<br>
É um dispositivo destinado à interrupção da operação em situações de emergência. Sua atuação é considerada na lógica de controle para priorizar a parada do sistema.<br>

• Sinalização Visual e Sonora<br>
O painel possui LEDs indicadores e sinalização sonora para auxiliar na identificação das condições de funcionamento do sistema. Esses recursos permitem demonstrar os estados de operação e as indicações previstas no projeto.<br>

• Motor Trifásico<br>
É o equipamento responsável por transformar energia elétrica em movimento mecânico. Seu sentido de rotação é controlado pelos contatores, de acordo com a sequência de fases estabelecida no circuito de potência.<br>

• Estrutura do Painel e Trilhos DIN<br>
A estrutura do painel serve como suporte para a instalação e organização dos componentes. Os trilhos DIN permitem a fixação de dispositivos como o CLP, os contatores, os disjuntores, a fonte de alimentação e os bornes de conexão, contribuindo para uma montagem organizada.<br>

Funcionamento Geral<br>
*Funcionamento do Sistema de Controle do Painel Didático*<br>

• Alimentação do Sistema<br>
O painel recebe alimentação de 220 VCA, utilizada no circuito de potência e na entrada da fonte de alimentação. A fonte converte a tensão para 24 VCC, utilizada na alimentação do CLP e do circuito de comando, conforme a configuração do projeto.<br>

• Envio dos Comandos<br>
O operador utiliza as botoeiras para solicitar a partida do motor em um dos sentidos de rotação ou para interromper seu funcionamento. O botão de emergência também fornece um comando prioritário de parada.<br>

• Processamento dos Sinais<br>
O CLP Siemens LOGO! recebe os sinais provenientes dos dispositivos de comando e executa a lógica programada em Ladder. Essa lógica determina quais saídas devem ser acionadas de acordo com os comandos recebidos e as condições de funcionamento do sistema.<br>

• Acionamento dos Contatores<br>
Quando a lógica de controle permite a partida, o CLP aciona o contator correspondente ao sentido de rotação solicitado. O KM1 estabelece a sequência de fases para um sentido, enquanto o KM2 inverte o sentido de rotação por meio da troca de duas fases.<br>

Os intertravamentos elétricos e lógicos impedem que os dois contatores sejam acionados simultaneamente, contribuindo para a segurança da operação.<br>

• Funcionamento do Motor<br>
O motor trifásico recebe alimentação por meio do circuito de potência e dos contatores. A combinação entre a sequência de fases e o contator acionado determina o sentido de rotação. Dessa forma, o sistema permite demonstrar a partida direta e a reversão do motor.<br>

• Parada, Emergência e Proteção<br>
O comando de parada interrompe a operação conforme a lógica programada. Em uma situação de emergência, o sistema prioriza o comando de interrupção. O disjuntor de proteção do motor também contribui para a segurança do circuito, e seu contato auxiliar pode ser utilizado para indicar uma condição de falha ao CLP.<br>

• Sinalização do Sistema<br>
As saídas do CLP controlam os indicadores luminosos e os recursos de sinalização sonora previstos no projeto. Esses dispositivos auxiliam na identificação das condições de operação e tornam o funcionamento do painel mais fácil de acompanhar durante as demonstrações didáticas.<br>

• Integração dos Sistemas
O funcionamento do painel depende da integração entre o circuito de potência, o circuito de comando e a programação do CLP. Os dispositivos de entrada fornecem os comandos, o controlador processa as informações e suas saídas acionam os contatores e os elementos de sinalização. Essa integração permite controlar o motor e demonstrar os princípios de automação industrial.<br>

• Resumo do Funcionamento<br>
O operador aciona uma botoeira → o CLP Siemens LOGO! recebe o comando → a lógica Ladder verifica as condições de operação e os intertravamentos → a saída correspondente aciona o contator KM1 ou KM2 → o circuito de potência alimenta o motor trifásico → o motor gira no sentido selecionado → os dispositivos de sinalização indicam as condições previstas no sistema.<br>

### Roteiro de Montagem

Para a montagem do painel didático, foram utilizadas ferramentas e instrumentos que auxiliaram na medição, fixação e instalação dos componentes elétricos. A trena foi empregada no dimensionamento dos trilhos DIN e das canaletas, enquanto a parafusadeira elétrica auxiliou na realização de furos e na fixação dos elementos estruturais.<br>
As chaves de fenda e Phillips foram utilizadas para apertar parafusos e fixar os componentes, e os alicates de corte e decapagem auxiliaram na preparação dos condutores elétricos para as conexões. Também foram utilizados terminais tubulares para facilitar a conexão e a organização dos fios nos pontos apropriados.<br>
A montagem envolveu a instalação do CLP Siemens LOGO!, dos contatores, dos disjuntores, da fonte de alimentação, dos bornes, das botoeiras e dos elementos de sinalização. Os componentes foram organizados na estrutura do painel, utilizando trilhos DIN e canaletas para auxiliar na disposição e no encaminhamento dos condutores.<br>
Após a instalação, foram realizadas as conexões dos circuitos de potência e comando com base nos diagramas elétricos do projeto. Em seguida, foram efetuados testes e ajustes para verificar a programação do CLP, o acionamento dos contatores, a reversão do motor e a atuação dos comandos de parada e emergência.<br>
Por fim, a documentação técnica e o manual do projeto foram elaborados para reunir informações e orientações sobre a montagem, as conexões elétricas, a programação e a operação do painel, contribuindo para a compreensão do sistema e sua utilização em atividades educacionais.<br>


### Montagem Final
A montagem final do painel didático de automação industrial envolveu a instalação e a organização dos componentes elétricos e de controle necessários para o funcionamento do sistema de partida direta com reversão de um motor trifásico. Para essa etapa, foram utilizadas ferramentas e instrumentos que auxiliaram na medição, fixação e conexão dos componentes, contribuindo para uma montagem organizada e adequada.<br>
A trena foi utilizada para medir e dimensionar os trilhos DIN e as canaletas, permitindo definir a disposição dos componentes no painel. A parafusadeira elétrica auxiliou na realização de furos e na fixação dos elementos estruturais, enquanto as chaves de fenda e Phillips foram empregadas no aperto dos parafusos e na fixação dos dispositivos elétricos.<br>
Também foram utilizados alicates de corte e decapagem para preparar os condutores elétricos, facilitando a realização das conexões entre os componentes. A estrutura de perfis de alumínio serviu como suporte para a montagem do painel, enquanto os trilhos DIN permitiram a instalação organizada dos disjuntores, da fonte de alimentação, do CLP Siemens LOGO!, dos contatores e dos bornes de conexão.<br>
Após a instalação dos componentes, foram realizadas as conexões dos circuitos de potência e comando, seguindo os diagramas elétricos elaborados durante o desenvolvimento do projeto. Em seguida, foram efetuados testes e ajustes para verificar o funcionamento da programação, o acionamento do motor nos dois sentidos de rotação e a atuação dos dispositivos de proteção, parada e emergência.<br>
Por fim, a documentação técnica e o manual do projeto reuniram orientações relacionadas à montagem, às conexões elétricas, à programação e à operação do painel, contribuindo para facilitar a compreensão do sistema e sua utilização em atividades didáticas de automação industrial. <br>

### Design Final

**• Conjunto Final Montado e Validado:<br>**
<img width="1200" height="1600" alt="Finalizado" src="https://github.com/user-attachments/assets/5d437c5b-1263-47c7-adff-4067e68cea0b" />


## 📅Cronograma
<img width="1133" height="944" alt="Gemini_Generated_Image_q3qm72q3qm72q3qm" src="https://github.com/user-attachments/assets/1773c8a3-256e-47a8-a3e3-f8abad4829e0" />

<span id="conclusao">
## ✅Conclusão
Com a finalização deste projeto, foi possível desenvolver um painel didático de partida direta com reversão de um motor trifásico, utilizando o CLP Siemens LOGO! para controlar o sistema por meio de uma programação em linguagem Ladder. O projeto teve como objetivo integrar os circuitos de potência e comando, os contatores, os dispositivos de proteção e os sistemas de sinalização, permitindo demonstrar o funcionamento do motor nos sentidos horário e anti-horário. Durante o desenvolvimento, foram realizadas pesquisas, seleção de componentes, elaboração de desenhos técnicos e diagramas elétricos, programação do CLP, montagem do painel e testes de funcionamento.<br>
Ao longo do processo, foram considerados desafios relacionados à disponibilidade de materiais e ao custo dos componentes necessários para a construção do painel. Essas limitações exigiram planejamento e análise na escolha dos materiais e na organização das etapas de desenvolvimento. Os testes realizados permitiram verificar o funcionamento dos comandos de acionamento, dos intertravamentos elétricos e lógicos e dos dispositivos de parada e emergência, contribuindo para avaliar a integração entre os circuitos elétricos e a programação do controlador.<br>
A colaboração entre os integrantes da equipe foi fundamental para a realização das atividades, possibilitando a divisão de responsabilidades, a troca de conhecimentos e a busca conjunta por soluções durante as etapas de planejamento, programação, montagem e testes. Além disso, o projeto proporcionou o aprimoramento de habilidades práticas relacionadas à montagem elétrica, à interpretação de diagramas, à programação de CLPs e à verificação do funcionamento de sistemas de automação industrial.<br>
Dessa forma, o desenvolvimento do painel didático contribuiu significativamente para a compreensão dos princípios de comandos elétricos e automação industrial, demonstrando a importância da integração entre hardware, circuitos elétricos e programação. A elaboração do relatório e do manual técnico, com orientações para montagem, conexões elétricas, programação e operação, complementou o trabalho e reuniu informações importantes para sua utilização didática e reprodução. Assim, o projeto reforçou a importância do planejamento, da organização, da segurança e do trabalho em equipe no desenvolvimento de soluções tecnológicas.<br>

> 

#### 📝Documentação:  [Clique Aqui](https://github.com/MavPro-tech/Painel_Didatico/tree/main/Sprints/Sprint_04)

<br>

  
  ---
  
</div>
