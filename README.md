# soc-detection-lab

Montagem de um centro de detecção em miniatura: um SIEM que coleta logs, ataques simulados contra máquinas próprias, regras de detecção escritas à mão e a triagem dos alertas mapeada no MITRE ATT&CK, fechando com um playbook de resposta.

> Projeto 5 de 7 do laboratório [sentinelatech](https://github.com/sentinelatech). Área: **SOC**.

## Por que isso importa em segurança

É a simulação mais fiel do trabalho de SOC de nível 1, a porta de entrada mais comum da área: receber alerta, decidir se é real, investigar e encaminhar. Fazer isso de ponta a ponta, inclusive escrevendo a regra que gera o alerta, mostra que você entende o ciclo inteiro.

## Objetivo

Com um SIEM próprio recebendo logs de um endpoint, simular algumas técnicas de ataque conhecidas, garantir que elas gerem alertas, triá-los como um analista faria e registrar o processo em um playbook.

## Estrutura

```
docs/especificacao.md   escopo e critério de aceite
docs/arquitetura.md     o desenho do lab e o fluxo de logs
deteccoes/              as regras de detecção escritas
relatorio/              triagem dos alertas e o mapeamento ATT&CK
playbook/               o passo a passo de resposta
```

## Laboratório

Wazuh (SIEM) em uma VM Linux e um endpoint monitorado (Windows com Sysmon, ou Linux) enviando logs. Em 12 GB livres, rode o Wazuh com uma VM de cada vez. Os ataques são simulados com ferramentas de emulação contra as suas próprias máquinas.

## Ferramentas

VirtualBox · Wazuh · Sysmon · MITRE ATT&CK · emulação de técnicas (por exemplo Atomic Red Team) contra as VMs do lab.

## Resultado

<!-- Preencher ao fim -->

## Aviso

Toda emulação de ataque ocorre entre máquinas virtuais próprias, isoladas. Nenhum sistema de terceiros é alvo.
