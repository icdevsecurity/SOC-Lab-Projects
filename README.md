# SOC-Lab-Projects
Laboratório prático de operações de segurança. Projetos de detecção de ameaças com SIEM, automação em Python e análise de logs. Portfolio para SOC analyst júnior.

# Projeto 1: Home SOC Lab

Laboratório de detecção de ameaças: simulo ataques com Atomic Red Team contra uma VM Windows, coleto os logs (Sysmon + Event Logs) e analiso no Splunk com queries SPL.

**Estrutura:**
- [documentacao](./projeto-1/documentacao): relatório com técnicas atacadas, logs gerados e queries usadas
- [screenshots](./projeto-1/screenshots): capturas do Splunk, dashboards e detecções
- [queries](./projeto-1/queries): queries SPL comentadas
- [logs](./projeto-1/logs): amostras dos logs coletados

**Limitações do ambiente:** uso Splunk Free (limite de 500 MB/dia), então os logs são enviados manualmente em lote, sem forwarder automático.
