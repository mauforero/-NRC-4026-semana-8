---
markmap:
  initialExpandLevel: 2
---

# Protocolo EIGRP

## Características

- Protocolo de estado de enlace
- Usa Algoritmo DUAL
- Autónomo en cada AS
- Soporta IPv4 e IPv6

## Configuración

- `router eigrp <AS>` → Activa EIGRP en el router
- `network <red> <wildcard>` → Configura redes EIGRP
- `passive-interface <int>` → Evita envíos innecesarios de paquetes EIGRP
- `show ip eigrp neighbors` → Verifica vecinos EIGRP

## Funcionamiento

- Calcula la mejor ruta basada en su métrica
- Detecta fallos rápidamente y adapta la topología
- Mantiene una tabla de topología con rutas alternativas

## Ventajas

- Convergencia rápida
- Bajo uso de ancho de banda
- Balanceo de carga desigual (Variance)
- Menos uso de CPU que OSPF

## Protocolos Similares

### EIGRP vs OSPF

- **EIGRP**: Más rápido en convergencia, usa métrica compuesta (ancho de banda, retardo, carga y confiabilidad).
- **OSPF**: Más escalable en redes grandes, usa métricas basadas en costo.

### EIGRP vs RIP

- **EIGRP**: Soporta balanceo de carga desigual y convergencia rápida.
- **RIP**: Lento en convergencia y usa solo el **número de saltos** como métrica.
