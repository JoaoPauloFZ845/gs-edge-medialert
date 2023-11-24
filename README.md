# MediAlert: Monitoramento de Saúde para Idosos

Integrantes:
João Paulo Fonseca Zamperlini RM99279
Matheus José de Lima Costa RM551157

## Descrição do Problema

O cuidado com a saúde de idosos é uma área que requer atenção especial, especialmente no que diz respeito à administração regular de medicamentos e ao risco de quedas. A aderência correta ao tratamento medicamentoso e a capacidade de responder rapidamente a emergências, como quedas, são fundamentais para garantir a segurança e o bem-estar dos idosos.

## Solução Proposta: MediAlert

O MediAlert é um projeto voltado para melhorar a gestão de medicamentos e aumentar a segurança dos idosos. A solução consiste em uma aplicação com duas interfaces distintas: uma simplificada para o usuário idoso e outra detalhada para o cuidador. As principais funcionalidades incluem:

- **Lembretes de Medicamentos**: Configuração de lembretes para a ingestão de medicamentos, com detalhes como nome, dosagem e horário.
- **Confirmação de Ingestão**: Capacidade do usuário confirmar a ingestão de medicamentos, informação que é compartilhada com o cuidador.
- **Botão de Emergência**: Um botão de emergência para enviar alertas imediatos aos cuidadores em situações críticas.
- **Sensor de Queda**: Um sensor acoplado a uma pulseira que detecta quedas e notifica automaticamente os cuidadores.
- **Relatórios Detalhados**: Geração de relatórios sobre a adesão aos medicamentos e incidentes para análise dos cuidadores e profissionais de saúde.

## Configuração e Execução

Para implementar a aprte de sensores do MediAlert, é necessário configurar um ESP32 com um botão e um acelerômetro. A montagem básica envolve:

1. **Montagem do Hardware**:
   - **ESP32**: O cérebro do sistema, responsável por processar os dados dos sensores e comunicar com a interface online.
   - **Botão de Emergência**: Conecte o botão a uma porta GPIO do ESP32. Este botão funcionará como um gatilho para enviar alertas.
   - **Acelerômetro**: Conecte um acelerômetro ao ESP32 para monitorar movimentos e detectar quedas.

2. **Configuração do Software**:
   - Programe o ESP32 para ler os dados do acelerômetro e monitorar o estado do botão de emergência.
   - Implemente a lógica para detectar quedas com base nos dados do acelerômetro.
   - Configure o ESP32 para enviar alertas para a interface online quando o botão de emergência for pressionado ou uma queda for detectada.

3. **Integração com a Interface Online**:
   - Estabeleça uma conexão entre o ESP32 e uma plataforma online (como o Wokwi) para visualizar e monitorar os dados em tempo real.

4. **Testes e Validação**:
   - Realize testes para garantir que o sistema detecta corretamente as quedas e que o botão de emergência está funcionando como esperado.
   - Valide a comunicação entre o ESP32 e a plataforma online, assegurando a transmissão correta dos dados.


Link para a simulação no Wokwi: https://wokwi.com/projects/382230574608615425

Link do Vídeo no Youtube: https://www.youtube.com/watch?v=1UhUYIF8Hm8&ab_channel=Jo%C3%A3oPauloZamperlini


O MediAlert é uma ferramenta essencial para a gestão da saúde de idosos, oferecendo tranquilidade aos usuários e seus cuidadores, além de facilitar a intervenção rápida em situações de emergência.
