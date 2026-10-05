# 📦 archive_eps_all_ana

[![Release](https://img.shields.io/github/v/release/34tm1d1ck/archive_eps_all_ana?label=release)](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest)

> ⬇️ **Get the files:** [Latest release](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest) · [Tagged assets](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/tag/embedded_software)

# 🚗 Nexteer Automotive — EPS All-in-One `(.7z)`

![Version](https://img.shields.io/badge/version-3.0-blue?style=flat-square)
![Size](https://img.shields.io/badge/size-6.7_GB-orange?style=flat-square)
![Files](https://img.shields.io/badge/files-24-green?style=flat-square)
![Format](https://img.shields.io/badge/format-.7z-lightgrey?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-yellow?style=flat-square)
![Platforms](https://img.shields.io/badge/platforms-RH850_%7C_TMS570-red?style=flat-square)

> `17x EPS` + `7x SIP Vector (BSW + Bootloader)` — ECU firmware, arch, models, validation, requirements.

## 📑 TOC

- [⚡ Quick Start](#-quick-start)
- [📦 What's Inside](#-whats-inside)
- [🔧 RH850 Firmware](#-rh850-firmware---4-packages)
- [⚙️ TMS570 Firmware](#️-tms570-firmware---9-packages)
- [📐 Arch / Models / Docs](#-arch--models--docs---5-packages)
- [🧪 Test / Requirements](#-test--requirements---2-packages)
- [📚 SIP Vector: BSW + Bootloader](#-sip-vector-bsw--bootloader---7-packages)
- [🗂️ Lookup Index](#️-lookup-index)
- [📄 License](#-license)

---

## ⚡ Quick Start

```bash
# List contents
7z l nexteer_automotive_ElectricPowerSteering_RH850_FORD_T3T6.7z

# Find code / config fast
rg -l "T1XX|FAAR|AUTOSAR|Bootloader" --glob '!*.7z'
```

> 💡 All archives are standalone. No inter-dependency. Pick by `MCU + OEM`.

[⬆ Back to top](#-nexteer-automotive--eps-all-in-one-7z)

---

## 📦 What's Inside

| # | Category | Count | Icon |
|---|----------|-------|------|
| 1 | 🔧 RH850 Firmware | 4 | Renesas RH850 |
| 2 | ⚙️ TMS570 Firmware | 9 | TI TMS570 |
| 3 | 📐 Arch / Models / Docs | 3 | Architecture + Simulink |
| 4 | 🧪 Test / Requirements | 2 | FIASA + VW RIF |
| 5 | 📚 BSW (AUTOSAR SIP) | 4 | Vector BSW |
| 6 | 🚀 Bootloader | 3 | Flash Bootloader |
| **Total** | | **24** | `6.7 GB` |

```text
./eps_all/
├── 🔧 rh850/          # 4x BMW, Ford, GM
├── ⚙️ tms570/         # 9x BMW, Chrysler, Fiat, GM, Haitec, PSA
├── 📐 arch_models/    # 3x Arch, Docs, Simulink
├── 🧪 test_req/       # 2x FIASA_CFG, VW_RIF
└── 📚 sip_vector/     # 4x BSW + 3x Bootloader
```

---

## 🔧 RH850 Firmware — 4 Packages

<details open>
<summary><b>Click to expand / collapse — 4x Renesas RH850</b></summary>

| OEM 🚗 | Archive 📦 | Scope 🎯 |
|---|---|---|
| BMW | `nexteer_automotive_ElectricPowerSteering_RH850_BMW_FAAR_WE.7z` | FAAR WE |
| Ford | `nexteer_automotive_ElectricPowerSteering_RH850_FORD_T3T6.7z` | T3T6 |
| GM | `nexteer_automotive_ElectricPowerSteering_RH850_GM_G2KCA.7z` | G2KCA |
| GM | `nexteer_automotive_ElectricPowerSteering_RH850_GM_T1XX.7z` | T1XX |

</details>

[⬆ Back to top](#-nexteer-automotive--eps-all-in-one-7z)

---

## ⚙️ TMS570 Firmware — 9 Packages

<details open>
<summary><b>Click to expand / collapse — 9x TI TMS570</b></summary>

| OEM 🚗 | Archive 📦 | Scope 🎯 |
|---|---|---|
| BMW | `nexteer_automotive_ElectricPowerSteering_TMS570_BMW_UKL_MCV.7z` | UKL MCV |
| Chrysler/Stellantis | `nexteer_automotive_ElectricPowerSteering_TMS570_CHRYSLER_LWR.7z` | LWR |
| Fiat | `nexteer_automotive_ElectricPowerSteering_TMS570_FIAT_321.7z` | 321 |
| GM | `nexteer_automotive_ElectricPowerSteering_TMS570_GM_9BXX.7z` | 9BXX |
| GM | `nexteer_automotive_ElectricPowerSteering_TMS570_GM_C1XX.7z` | C1XX |
| Haitec | `nexteer_automotive_ElectricPowerSteering_TMS570_HAITEC_LC.7z` | LC |
| PSA | `nexteer_automotive_ElectricPowerSteering_TMS570_PSA_BMPV.7z` | BMPV |
| PSA | `nexteer_automotive_ElectricPowerSteering_TMS570_PSA_CMP.7z` | CMP |
| — | _+ GM 9BXX listed in requirements group, same MCU_ | — |

> ℹ️ For `9BXX / C1XX / BMPV / CMP`: same MCU, different calibration.

</details>

[⬆ Back to top](#-nexteer-automotive--eps-all-in-one-7z)

---

## 📐 Arch / Models / Docs — 3 Packages

<details>
<summary><b>Click to expand — Architecture + Simulink + Docs</b></summary>

| Type | Archive 📦 | Use For 💻 |
|---|---|---|
| 🏛️ Arch | `nexteer_automotive_SoftwareArchitecture_EPS_BMW.7z` | BMW FAAR WE SW arch — interfaces, components |
| 📊 Models | `nexteer_automotive_ModelBasedDesignSimulink.7z` | Simulink + Embedded Coder examples |
| 📖 Docs | `nexteer_automotive_ElectricPowerSteering_Documentation.7z` | Core EPS design refs |

```bash
# Open Simulink models
matlab -r "open('./ModelBasedDesignSimulink')"
```

</details>

---

## 🧪 Test / Requirements — 2 Packages

<details>
<summary><b>Click to expand — Validation + OEM Requirements</b></summary>

| Type | Archive 📦 | Notes 📝 |
|---|---|---|
| 🧪 Test CFG | `nexteer_automotive_FIASA_TEST_CFG.7z` | Fiat EPS validation env |
| 📋 Reqs | `nexteer_automotive_Volkswagen_EPS_Requirements_RIF.7z` | VW DOORS RIF — import to DOORS / ReqM2 |

```bash
# RIF import hint (DOORS / Python)
python -c "import xml.etree.ElementTree as ET; print(ET.parse('vw_eps.rif').getroot().tag)"
```

</details>

[⬆ Back to top](#-nexteer-automotive--eps-all-in-one-7z)

---

## 📚 SIP Vector: BSW + Bootloader — 7 Packages

<details open>
<summary><b>Click to expand / collapse — AUTOSAR BSW + FBL</b></summary>

### 🧩 AUTOSAR BSW (4x)

| MCU | Archive 📦 | OEM | Size 💾 |
|---|---|---|---|
| RH850 | `nexteer_automotive_BSW_RH850_BMW.7z` | BMW | 572 MB |
| RH850 | `nexteer_automotive_BSW_RH850_FCA.7z` | FCA | 420 MB |
| RH850 | `nexteer_automotive_BSW_RH850_FORD.7z` | Ford | 509 MB |
| TMS570 | `nexteer_automotive_BSW_TMS570_PSA.7z` | PSA | 35.5 MB |

### 🚀 Flash Bootloader (3x)

| MCU | Archive 📦 | OEM | Size 💾 |
|---|---|---|---|
| RH850 | `nexteer_automotive_FlashBootloader_RH850_Generic.7z` | Generic | 13 MB |
| RH850 | `nexteer_automotive_FlashBootloader_RH850_GM.7z` | GM | 18.8 MB |
| TMS570 | `nexteer_automotive_FlashBootloader_TMS570_GM.7z` | GM | 13.2 MB |

</details>

[⬆ Back to top](#-nexteer-automotive--eps-all-in-one-7z)

---

## 🗂️ Lookup Index

> 🔍 `Ctrl+F` cheatsheet — `MCU → OEM → file`.

| 🔎 Search | 📦 File |
|---|---|
| `BMW FAAR` | `..._RH850_BMW_FAAR_WE.7z` + `..._SoftwareArchitecture_EPS_BMW.7z` |
| `BMW UKL` | `..._TMS570_BMW_UKL_MCV.7z` |
| `Ford` | `..._RH850_FORD_T3T6.7z` + `..._BSW_RH850_FORD.7z` |
| `GM T1XX / G2KCA` | `..._RH850_GM_T1XX.7z` / `..._RH850_GM_G2KCA.7z` |
| `GM C1XX / 9BXX` | `..._TMS570_GM_C1XX.7z` / `..._TMS570_GM_9BXX.7z` |
| `FCA` | `..._BSW_RH850_FCA.7z` |
| `PSA` | `..._TMS570_PSA_CMP.7z` / `..._TMS570_PSA_BMPV.7z` / `..._BSW_TMS570_PSA.7z` |
| `Fiat / Chrysler` | `..._TMS570_FIAT_321.7z` / `..._TMS570_CHRYSLER_LWR.7z` / `..._FIASA_TEST_CFG.7z` |
| `VW` | `..._Volkswagen_EPS_Requirements_RIF.7z` |
| `Simulink` | `..._ModelBasedDesignSimulink.7z` |
| `FBL` | `..._FlashBootloader_*.7z` (x3) |

- ✅ Pick by filename: `{EPS|BSW|FlashBootloader}_{MCU}_{OEM}_{PLATFORM}.7z`
- ✅ RH850 = Renesas, TMS570 = TI
- ✅ RIF = DOORS XML, Simulink = `.slx` + Embedded Coder

---

## 📄 License

`MIT` — see `LICENSE` in repo root.

```
SPDX-License-Identifier: MIT
```

---
<div align="center">

**🚗 Nexteer EPS `v3.0` — 24 archives — `6.7 GB`**

[⚡ Quick Start](#-quick-start) • [📦 Contents](#-whats-inside) • [🔧 RH850](#-rh850-firmware---4-packages) • [⚙️ TMS570](#️-tms570-firmware---9-packages) • [📚 SIP](#-sip-vector-bsw--bootloader---7-packages)

</div>

---

## ⬇️ Downloads (latest, auto-generated)

Base: `https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/<asset>`

| Archive 📦 | Size 💾 | Download 🔗 |
|---|---|---|
| `nexteer_automotive_BSW_RH850_BMW.7z` | 572M | [⬇️ nexteer_automotive_BSW_RH850_BMW.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_BSW_RH850_BMW.7z) |
| `nexteer_automotive_BSW_RH850_FCA.7z` | 421M | [⬇️ nexteer_automotive_BSW_RH850_FCA.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_BSW_RH850_FCA.7z) |
| `nexteer_automotive_BSW_RH850_FORD.7z` | 510M | [⬇️ nexteer_automotive_BSW_RH850_FORD.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_BSW_RH850_FORD.7z) |
| `nexteer_automotive_BSW_TMS570_PSA.7z` | 36M | [⬇️ nexteer_automotive_BSW_TMS570_PSA.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_BSW_TMS570_PSA.7z) |
| `nexteer_automotive_ElectricPowerSteering_Documentation.7z` | 80M | [⬇️ nexteer_automotive_ElectricPowerSteering_Documentation.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_Documentation.7z) |
| `nexteer_automotive_ElectricPowerSteering_RH850_BMW_FAAR_WE.7z` | 1.1G | [⬇️ nexteer_automotive_ElectricPowerSteering_RH850_BMW_FAAR_WE.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_RH850_BMW_FAAR_WE.7z) |
| `nexteer_automotive_ElectricPowerSteering_RH850_FORD_T3T6.7z` | 1.5G | [⬇️ nexteer_automotive_ElectricPowerSteering_RH850_FORD_T3T6.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_RH850_FORD_T3T6.7z) |
| `nexteer_automotive_ElectricPowerSteering_RH850_GM_G2KCA.7z` | 1.3G | [⬇️ nexteer_automotive_ElectricPowerSteering_RH850_GM_G2KCA.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_RH850_GM_G2KCA.7z) |
| `nexteer_automotive_ElectricPowerSteering_RH850_GM_T1XX.7z` | 1.3G | [⬇️ nexteer_automotive_ElectricPowerSteering_RH850_GM_T1XX.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_RH850_GM_T1XX.7z) |
| `nexteer_automotive_ElectricPowerSteering_TMS570_BMW_UKL_MCV.7z` | 35M | [⬇️ nexteer_automotive_ElectricPowerSteering_TMS570_BMW_UKL_MCV.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_TMS570_BMW_UKL_MCV.7z) |
| `nexteer_automotive_ElectricPowerSteering_TMS570_CHRYSLER_LWR.7z` | 272M | [⬇️ nexteer_automotive_ElectricPowerSteering_TMS570_CHRYSLER_LWR.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_TMS570_CHRYSLER_LWR.7z) |
| `nexteer_automotive_ElectricPowerSteering_TMS570_FIAT_321.7z` | 479M | [⬇️ nexteer_automotive_ElectricPowerSteering_TMS570_FIAT_321.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_TMS570_FIAT_321.7z) |
| `nexteer_automotive_ElectricPowerSteering_TMS570_GM_9BXX.7z` | 1.7M | [⬇️ nexteer_automotive_ElectricPowerSteering_TMS570_GM_9BXX.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_TMS570_GM_9BXX.7z) |
| `nexteer_automotive_ElectricPowerSteering_TMS570_GM_C1XX.7z` | 524M | [⬇️ nexteer_automotive_ElectricPowerSteering_TMS570_GM_C1XX.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_TMS570_GM_C1XX.7z) |
| `nexteer_automotive_ElectricPowerSteering_TMS570_HAITEC_LC.7z` | 360M | [⬇️ nexteer_automotive_ElectricPowerSteering_TMS570_HAITEC_LC.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_TMS570_HAITEC_LC.7z) |
| `nexteer_automotive_ElectricPowerSteering_TMS570_PSA_BMPV.7z` | 435M | [⬇️ nexteer_automotive_ElectricPowerSteering_TMS570_PSA_BMPV.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_TMS570_PSA_BMPV.7z) |
| `nexteer_automotive_ElectricPowerSteering_TMS570_PSA_CMP.7z` | 570M | [⬇️ nexteer_automotive_ElectricPowerSteering_TMS570_PSA_CMP.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ElectricPowerSteering_TMS570_PSA_CMP.7z) |
| `nexteer_automotive_FIASA_TEST_CFG.7z` | 3.7M | [⬇️ nexteer_automotive_FIASA_TEST_CFG.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_FIASA_TEST_CFG.7z) |
| `nexteer_automotive_FlashBootloader_RH850_GM.7z` | 20M | [⬇️ nexteer_automotive_FlashBootloader_RH850_GM.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_FlashBootloader_RH850_GM.7z) |
| `nexteer_automotive_FlashBootloader_RH850_Generic.7z` | 14M | [⬇️ nexteer_automotive_FlashBootloader_RH850_Generic.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_FlashBootloader_RH850_Generic.7z) |
| `nexteer_automotive_FlashBootloader_TMS570_GM.7z` | 14M | [⬇️ nexteer_automotive_FlashBootloader_TMS570_GM.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_FlashBootloader_TMS570_GM.7z) |
| `nexteer_automotive_ModelBasedDesignSimulink.7z` | 15M | [⬇️ nexteer_automotive_ModelBasedDesignSimulink.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_ModelBasedDesignSimulink.7z) |
| `nexteer_automotive_SoftwareArchitecture_EPS_BMW.7z` | 6.0M | [⬇️ nexteer_automotive_SoftwareArchitecture_EPS_BMW.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_SoftwareArchitecture_EPS_BMW.7z) |
| `nexteer_automotive_Volkswagen_EPS_Requirements_RIF.7z` | 9.0M | [⬇️ nexteer_automotive_Volkswagen_EPS_Requirements_RIF.7z](https://github.com/34tm1d1ck/archive_eps_all_ana/releases/latest/download/nexteer_automotive_Volkswagen_EPS_Requirements_RIF.7z) |
