# Especificação — soc-detection-lab

**Semana:** 20/11 a 26/11/2026
**Entrega final:** regras de detecção + relatório de triagem + playbook

## Contexto

O time montou um SOC pequeno e você é o analista. Precisa garantir que ataques comuns gerem alerta, saber triar o que aparece e deixar um playbook para que outra pessoa consiga responder do mesmo jeito.

## Escopo

1. **Subir o SIEM** — Wazuh em uma VM, com um endpoint enviando logs (Sysmon no Windows, ou logs do Linux).
2. **Simular ataques** — emular ao menos três técnicas conhecidas do ATT&CK contra as suas VMs (por exemplo: força bruta, execução suspeita, persistência).
3. **Detectar** — garantir que cada técnica gere alerta; onde não gerar, escrever a regra de detecção.
4. **Triar** — para cada alerta: é real ou falso positivo? Qual a evidência? Qual a técnica ATT&CK? Qual a gravidade?
5. **Responder** — um playbook com os passos de contenção e investigação para o tipo de alerta mais relevante.

## Critério de aceite

- [ ] Arquitetura do lab documentada (`docs/arquitetura.md`)
- [ ] Três técnicas simuladas, cada uma mapeada ao ATT&CK
- [ ] Ao menos uma regra de detecção escrita por você, versionada em `deteccoes/`
- [ ] Relatório de triagem com evidência por alerta
- [ ] Playbook de resposta reproduzível
- [ ] README com o resultado em uma linha

## Fora de escopo

Qualquer emulação fora das VMs do laboratório.

## Fases (issues da semana)

| Dia | Fase | Entrega do dia |
|---|---|---|
| Sex 20/11 | Subir o Wazuh e ligar o endpoint | SIEM recebendo logs |
| Sáb 21/11 | Primeira técnica e alerta (dia leve) | Alerta gerado e triado |
| Dom 22/11 | Segunda técnica e alerta (dia leve) | Alerta mapeado ao ATT&CK |
| Seg 23/11 | Terceira técnica e regra própria | Regra de detecção em `deteccoes/` |
| Ter 24/11 | Relatório de triagem | Triagem dos três alertas em rascunho |
| Qua 25/11 | Playbook de resposta | `playbook/` reproduzível |
| Qui 26/11 | Fechamento | Relatório final, arquitetura e README |
