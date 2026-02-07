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

## 40 — Accesibil

