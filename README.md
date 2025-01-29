<div align="right">
  <a href="#portugues"><button>Português</button></a>
  <a href="#english"><button>English</button></a>
</div>

# <a name="portugues"></a> Template de Monitoramento

Um modelo abrangente para monitoramento de dispositivos, com foco em aspectos de saúde, rede, sistema, armazenamento e CPU. Este template inclui uma variedade de itens, triggers e regras de descoberta para coletar e apresentar informações detalhadas sobre os dispositivos monitorados.

## Itens Monitorados
- **ICMP Ping:** Monitora a disponibilidade do dispositivo através de pings ICMP.
- **Perda de Pacotes ICMP:** Acompanha a porcentagem de pacotes ICMP perdidos.
- **Tempo de Resposta ICMP:** Mede o tempo de resposta dos pings ICMP.
- **SNMP Walk para Interfaces de Rede:** Descobre e monitora interfaces de rede através de SNMP.
- **SNMP Traps (fallback):** Coleta traps SNMP não correspondidas por outros itens.
- **Detalhes de Contato do Sistema:** Obtém informações de contato do sistema via SNMP.
- **SNMP Walk para CPUs:** Descobre e monitora as CPUs do sistema.
- **Descrição do Sistema:** Coleta a descrição do sistema através de SNMP.
- **Modelo de Hardware:** Obtém o modelo de hardware do dispositivo via SNMP.
- **Uptime (Hardware):** Monitora o tempo desde a última inicialização do hardware.
- **Localização do Sistema:** Coleta a localização física do dispositivo.
- **Nome do Sistema:** Obtém o nome do sistema.
- **Uptime (Rede):** Mede o tempo desde a última reinicialização da parte de gerenciamento de rede do sistema.
- **ID do Objeto do Sistema:** Coleta o identificador do subsistema de gerenciamento de rede do dispositivo.
- **SNMP Walk para Sistemas de Arquivos Montados:** Descobre e monitora sistemas de arquivos montados.
- **Memória Total:** Monitora a quantidade total de memória disponível.
- **Disponibilidade do Agente SNMP:** Verifica se o agente SNMP está disponível.

## Regras de Descoberta
- **Descoberta de CPU:** Descobre e monitora a utilização da CPU através de SNMP.
- **Descoberta de Interfaces de Rede:** Descobre e monitora interfaces de rede com base em vários filtros.
- **Descoberta de Armazenamento:** Descobre e monitora o uso do espaço em disco.

## Triggers
- **Disponibilidade:** Detecta indisponibilidade via ICMP ou SNMP.
- **Desempenho:** Identifica alta perda de pacotes ICMP e alta utilização da CPU.
- **Capacidade:** Detecta espaço em disco criticamente baixo.
- **Notificações:** Detecta mudanças no nome do sistema e reinicializações.
- **Erros:** Identifica erros nas interfaces de rede.

## Outros
- Inclui dashboards para visualizar informações sobre interfaces de rede.
- Utiliza macros para configurar limiares e filtros.
- Baseado no template **MikroTik hEX by SNMP** do Zabbix.

---

# <a name="english"></a> Monitoring Template

A comprehensive template for monitoring devices, focusing on health, network, system, storage, and CPU aspects. This template includes various items, triggers, and discovery rules to collect and present detailed information about monitored devices.

## Monitored Items
- **ICMP Ping:** Monitors device availability via ICMP pings.
- **ICMP Packet Loss:** Tracks the percentage of lost ICMP packets.
- **ICMP Response Time:** Measures ICMP ping response time.
- **SNMP Walk for Network Interfaces:** Discovers and monitors network interfaces via SNMP.
- **SNMP Traps (fallback):** Collects SNMP traps not matched by other items.
- **System Contact Details:** Retrieves system contact information via SNMP.
- **SNMP Walk for CPUs:** Discovers and monitors system CPUs.
- **System Description:** Collects system description via SNMP.
- **Hardware Model:** Retrieves the device's hardware model via SNMP.
- **Uptime (Hardware):** Monitors the time since the last hardware startup.
- **System Location:** Collects the physical location of the device.
- **System Name:** Retrieves the system name.
- **Uptime (Network):** Measures the time since the last restart of the network management system.
- **System Object ID:** Collects the identifier of the network management subsystem.
- **SNMP Walk for Mounted File Systems:** Discovers and monitors mounted file systems.
- **Total Memory:** Monitors the total available memory.
- **SNMP Agent Availability:** Checks if the SNMP agent is available.

## Discovery Rules
- **CPU Discovery:** Discovers and monitors CPU usage via SNMP.
- **Network Interface Discovery:** Discovers and monitors network interfaces based on multiple filters.
- **Storage Discovery:** Discovers and monitors disk space usage.

## Triggers
- **Availability:** Detects unavailability via ICMP or SNMP.
- **Performance:** Identifies high ICMP packet loss and high CPU usage.
- **Capacity:** Detects critically low disk space.
- **Notifications:** Detects system name changes and host reboots.
- **Errors:** Identifies errors on network interfaces.

## Others
- Includes dashboards for visualizing network interface information.
- Uses macros to configure thresholds and filters.
- Based on the **MikroTik hEX by SNMP** template from Zabbix.

