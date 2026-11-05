# Laboratório 02 — Configuração Básica de Switch Cisco

## Objetivo
Configurar um switch Cisco 2960 e estabelecer comunicação entre dois computadores utilizando o Cisco Packet Tracer.

## Equipamentos
- 1 switch Cisco 2960
- 2 computadores
- 2 cabos Copper Straight-Through

## Endereçamento IPv4

| Dispositivo | Endereço IP | Máscara |
|---|---|---|
| PC-01 | 192.168.10.10 | 255.255.255.0 |
| PC-02 | 192.168.10.20 | 255.255.255.0 |

## Configuração do switch

```text
enable
configure terminal
hostname SW-01
interface fastEthernet 0/1
description CONEXAO-PC01
no shutdown
exit
interface fastEthernet 0/2
description CONEXAO-PC02
no shutdown
end
show running-config
copy running-config startup-config
```

## Teste de conectividade

Comando executado no PC-01:

```text
ping 192.168.10.20
```

**Resultado:** 4 pacotes enviados, 4 recebidos e 0% de perda.

## Conhecimentos adquiridos

- Configuração básica de switches Cisco
- Navegação pela CLI do Cisco IOS
- Configuração de interfaces
- Endereçamento IPv4
- Diagnóstico de conectividade
- Salvamento de configurações

## Conclusão

O laboratório foi concluído com sucesso, demonstrando comunicação entre dois computadores conectados a um switch Cisco 2960.

Projeto desenvolvido durante minha preparação para a certificação Cisco CCNA 200-301.
