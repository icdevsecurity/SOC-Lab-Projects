# SOC-Lab-Projects
Laboratório prático de operações de segurança. Projetos de detecção de ameaças com SIEM, automação em Python e análise de logs. Portfolio para SOC analyst júnior.

## Projeto 1: Laboratório SOC Doméstico

Laboratório de detecção de ameaças: simulo ataques com Atomic Red Team contra uma VM Windows, coleto os logs (Sysmon + Event Logs) e analiso no Splunk com consultas SPL.

**Ferramentas:** Atomic Red Team, Sysmon, Windows Event Logs, Splunk Free, [MITRE ATT&CK](https://attack.mitre.org/)

**Estrutura:**
- [documentação](./projeto-1/documentacao): relatório com técnicas de ataque (mapeadas ao MITRE ATT&CK), logs gerados e consultas usadas
- [capturas de tela](./projeto-1/screenshots): capturas do Splunk, dashboards e detecções
- [consultas](./projeto-1/queries): consultas SPL comentadas
- [logs](./projeto-1/logs): amostras dos logs coletados

**O que este projeto demonstra:**
- Análise de logs do Windows (Sysmon e Event Logs)
- Criação de consultas SPL para detectar comportamento malicioso
- Mapeamento de ataques ao MITRE ATT&CK e detecção baseada em comportamento

**Limitações do ambiente:** uso Splunk Free (limite de 500 MB/dia), então os logs são enviados manualmente em lote, sem forwarder automático.

## Projeto 2: Detecção de Força Bruta

Ataque de força bruta com Hydra/Medusa (Kali) contra RDP/SMB de uma VM Windows, e detecção no Splunk por múltiplas falhas de login (Event ID 4625) seguidas de sucesso (4624).

**Ferramentas:** Kali Linux, Hydra/Medusa, Splunk Free, Windows Event Logs, [MITRE ATT&CK](https://attack.mitre.org/)

**Estrutura:**
- [documentação](./projeto-2/documentacao): relatório do ataque, logs gerados e lógica de detecção
- [capturas de tela](./projeto-2/capturas-de-tela): ataque em execução e detecção no Splunk
- [consultas](./projeto-2/consultas): consultas SPL comentadas
- [logs](./projeto-2/logs): amostras dos logs coletados

**O que este projeto demonstra:**
- Escrita de regra de detecção (não só execução de ferramenta)
- Correlação de eventos 4625 → 4624
- Análise de logs de autenticação do Windows

---

## Projeto 3: Análise de Tráfego Malicioso com Wireshark

Análise de PCAPs de malware (ex: malware-traffic-analysis.net) e de tráfego gerado no laboratório, identificando beaconing, exfiltração de dados e DNS suspeito. O resultado é um relatório de análise de tráfego no formato de entrega a um cliente.

**Ferramentas:** Wireshark, PCAPs públicos, Kali Linux

**Estrutura:**
- [documentação](./projeto-3/documentacao): relatório de análise de tráfego
- [capturas de tela](./projeto-3/capturas-de-tela): evidências no Wireshark
- [filtros](./projeto-3/filtros): filtros do Wireshark usados, comentados
- [indicadores](./projeto-3/indicadores): IOCs encontrados (IPs, domínios, hashes)

**O que este projeto demonstra:**
- Análise de pacotes e identificação de comportamento malicioso
- Detecção de beaconing, exfiltração e DNS suspeito
- Comunicação técnica para público externo

---

## Projeto 4: Simulação de Ataque Mapeado no MITRE ATT&CK

Execução de técnicas específicas (ex: T1110 Brute Force, T1046 Network Service Discovery) com o Kali, captura no Wireshark e detecção no Splunk, consolidadas em uma tabela de rastreabilidade.

| Técnica MITRE | Ferramenta usada | Log gerado | Query de detecção |
|---|---|---|---|
| T1110 Brute Force | (preencher) | (preencher) | (preencher) |
| T1046 Network Service Discovery | (preencher) | (preencher) | (preencher) |

**Estrutura:**
- [documentação](./projeto-4/documentacao): relatório completo com a tabela e a análise
- [capturas de tela](./projeto-4/capturas-de-tela): evidências do Wireshark e do Splunk
- [consultas](./projeto-4/consultas): consultas SPL comentadas
- [logs](./projeto-4/logs): amostras dos logs coletados

**O que este projeto demonstra:**
- Mapeamento de ataque ao MITRE ATT&CK
- Ciclo completo: ataque → captura → detecção
- Documentação de cobertura de detecção
