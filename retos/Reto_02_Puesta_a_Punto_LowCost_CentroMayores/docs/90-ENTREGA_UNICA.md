# Reto 02 — Puesta a Punto Low-Cost y Competitiva
UT3 · RA1 — Centro de Mayores

---

## 10 — Diagnóstico inicial del lote

### Muestra de 5 unidades

| Equipo | CPU | RAM | Almacenamiento | Observaciones |
|------|-----|-----|----------------|---------------|
| A | Intel Core 2 Duo E8400 | 4 GB DDR3 | HDD 160 GB | Arranque lento, HDD antiguo |
| B | Intel Core i3-2100 | 4 GB DDR3 | HDD 250 GB | HDD ruidoso |
| C | AMD Athlon X2 | 4 GB DDR2 | HDD 250 GB | Temperatura elevada |
| D | Pentium Dual Core E5400 | 4 GB DDR3 | HDD 160 GB | Sectores reasignados |
| E | Core 2 Quad Q6600 | 8 GB DDR3 | HDD 320 GB | Estable |

**Estado térmico (aprox.):**
- Reposo: 45–55 °C  
- Carga breve: 70–80 °C  

**Problemas detectados:**
- HDD mecánicos lentos
- Ruido y vibraciones
- RAM limitada para uso web moderno

---

## 20 — Selección de SO ligero

| Distro | Requisitos | Soporte | Pros | Contras | Decisión |
|------|-----------|---------|------|---------|---------|
| Xubuntu LTS | 1.5 GB RAM | Muy bueno | Ligero, estable | UI simple | ✅ Elegido |
| Lubuntu | 1 GB RAM | Bueno | Muy rápido | UI básica | Alternativa |
| Linux Mint XFCE | 2 GB RAM | Excelente | Muy amigable | Algo más pesado | Descartado |

**Decisión:** Xubuntu LTS.

---

## 30 — Instalación y post-instalación

**Pasos:**
1. USB booteable con Xubuntu
2. Instalación limpia
3. Usuario estándar
4. Actualizaciones automáticas

**Paquetes esenciales:**
- Firefox
- LibreOffice
- VLC
- Codecs multimedia

**Usuarios y políticas:**
- Usuario sin privilegios
- Sudo solo bajo demanda

---

## 40 — Accesibilidad para mayores

- Escala UI 130 %
- Tema claro y alto contraste
- Accesos directos grandes a:
  - Correo web
  - Videollamadas
  - Ofimática online
- Ratón con velocidad reducida
- Doble clic desactivado

---

## 50 — Optimización de rendimiento

- zRAM activado
- Swapfile 2 GB
- Servicios innecesarios deshabilitados
- Navegador optimizado con bloqueo de anuncios

---

## 60 — Seguridad básica

- Usuario estándar
- Firewall UFW activo
- Actualizaciones automáticas
- Restauración con Timeshift

---
# 65 — Análisis de mercado y PVP objetivo

| Plataforma     | Enlace                                                                                                                                                       |                         | Precio (€)                   | Especificación clave                      |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------- | ---------------------------- | ----------------------------------------- |
| Wallapop       | [https://www.wallapop.com/item/ordenador-de-sobremesa-802487824](https://www.wallapop.com/item/ordenador-de-sobremesa-802487824)                             | | 150 €                        | Intel Core Quad + SSD 240 GB + 4 GB RAM   |
| eBay           | [https://www.ebay.es/b/Ordenadores-de-sobremesa/171957/bn_16553696](https://www.ebay.es/b/Ordenadores-de-sobremesa/171957/bn_16553696)                       || ~180–260 €                   | Dell/Lenovo / 8–16 GB RAM / SSD (usado)   |
| CashConverters | [https://www.cashconverters.es/es/es/comprar/informatica/ordenador-sobremesa/](https://www.cashconverters.es/es/es/comprar/informatica/ordenador-sobremesa/) || ~240–300+ € (segmento común) | Ordenadores reacondicionados con garantía |

> Reglas de captura: URL completa visible + fecha/hora del sistema visibles + dato marcado.

2) PVP objetivo y criterio de competitividad

**Precio medio comparables (estimado):**

Wallapop: ~150 €

eBay: ~220 €

CashConverters: ~270 €
**Precio medio simple:**

Precio medio simple:

(150+220+270)/3
	​

=213,33 €

**PVP objetivo por unidad: ≈ 200 €**

**Criterio de competitividad:**
Coste total por unidad ≤ Precio comparable medio − 15 %

200€×(1−0.15)=170€

Este margen del 15 % permite posicionarse claramente por debajo del mercado, ofreciendo un valor más atractivo para el cliente final.

## 70 — Métricas antes/después

| Métrica | Antes | Después |
|------|-------|---------|
| Arranque | 120 s | 35 s |
| RAM en reposo | 1200 MB | 850 MB |
| CPU YouTube 720p | 70 % | 30 % |
| Temp. en carga | 78 °C | 68 °C |

---

## 75 — Presupuesto de hardware y ROI

### Escenarios

| Escenario | Gasto HW | Horas | Tarifa €/h | Coste total | PVP | ROI |
|---------|----------|-------|------------|-------------|-----|-----|
| S0 | 0 € | 3 | 15 € | 65 € | 70 € | 0.08 |
| S1 | 15 € | 4 | 15 € | 95 € | 120 € | 0.26 |
| S2 | 30 € | 5 | 15 € | 155 € | 150 € | -0.03 |

**Escenario elegido:** S1  

**Motivos:**
- Gran mejora de rendimiento con bajo coste
- Muy competitivo en mercado de segunda mano
- ROI positivo

---

## 80 — Replicación en flota

- Imagen base con Clonezilla
- Restauración masiva
- Verificación checksum
- Cambio de hostname tras clonación

---

## 85 — Plan de mantenimiento

- Limpieza física cada 6 meses
- Revisión SMART trimestral
- Actualizaciones semanales
- Copias con Timeshift

---

