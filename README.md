# SOC-Lab-Projects
Laboratório prático de operações de segurança. Projetos de detecção de ameaças com SIEM, automação em Python e análise de logs. Portfolio para SOC analyst júnior.

## Projeto 1: Laboratório SOC Doméstico

Laboratório de detecção de ameaças: simulo ataques com Atomic Red Team contra uma VM Windows, coleto os logs (Sysmon + Event Logs) e analiso no Splunk com consultas SPL.

**Ferramentas:** Atomic Red Team, Sysmon, Windows Event Logs, Splunk Free, [MITRE ATT&CK](https://attack.mitre.org/)

**Estrutura:**
- [documentação](./projeto-1/documentacao): relatório com técnicas atacadas (mapeadas ao MITRE ATT&CK), logs gerados e consultas usadas
- [capturas de tela](./projeto-1/screenshots): capturas do Splunk, dashboards e detecções
- [consultas](./projeto-1/queries): consultas SPL comentadas
- [logs](./projeto-1/logs): amostras dos logs coletados

**O que este projeto demonstra:**
- Análise de logs do Windows (Sysmon e Event Logs)
- Criação de consultas SPL para detectar comportamento malicioso
- Mapeamento de ataques ao MITRE ATT&CK e detecção baseada em comportamento

**Limitações do ambiente:** uso Splunk Free (limite de 500 MB/dia), então os logs são enviados manualmente em lote, sem forwarder automático.
