# 🛡️ SNORT 2.9.16 가이드 (KOR)
> **SNORT 2.9.16 공식 매뉴얼 기반 한국어 규칙 가이드입니다.**

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![SNORT Version](https://img.shields.io/badge/SNORT-2.9.16-red.svg)](https://www.snort.org/)
[![Author](https://img.shields.io/badge/Author-BentLock-orange.svg)](https://github.com/BentLock)

---

## Contents
- [3. Writing Snort Rules](./3.-Writing_Snort_Rules/README.md)
	- [3.1 The Basics](./3.-Writing_Snort_Rules/3.1-The_Basics.md)
	- [3.2 Rules Headers](./3.-Writing_Snort_Rules/3.2-Rules_Headers.md)
		- [3.2.1 Action](./3.-Writing_Snort_Rules/3.2-Rules_Headers.md#321-action)
		- [3.2.2 Protocols](./3.-Writing_Snort_Rules/3.2-Rules_Headers.md#322-protocols)
		- [3.2.3 IP Addresses](./3.-Writing_Snort_Rules/3.2-Rules_Headers.md#323-ip-addresses)
		- [3.2.4 Port Numbers](./3.-Writing_Snort_Rules/3.2-Rules_Headers.md#324-port-numbers)
		- [3.2.5 The Direction Operator](./3.-Writing_Snort_Rules/3.2-Rules_Headers.md#325-the-direction-operator)
		- [3.2.6 Activate/Dynamic Rules](./3.-Writing_Snort_Rules/3.2-Rules_Headers.md#326-activatedynamic-rules)
	- [3.3 Rule Options](./3.-Writing_Snort_Rules/3.3-Rule_Options.md)
	- [3.4 General Rule Options](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md)
		- [3.4.1 msg](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#341-msg)
		- [3.4.2 reference](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#342-reference)
		- [3.4.3 gid](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#343-gid)
		- [3.4.4 sid](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#344-sid)
		- [3.4.5 rev](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#345-rev)
		- [3.4.6 classtype](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#346-classtype)
		- [3.4.7 priority](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#347-priority)
		- [3.4.8 metadata](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#348-metadata)
		- [3.4.9 General Rule Options](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md/#349-general-rule-quick-reference)
	- [3.5 Payload Detection Rule Options](./3.-Writing_Snort_Rules/3.5-Payload-Detection-Rule-Options.md)

---

### 📜 라이선스 요약 (License Summary)

1. **Analysis & Summary (By BentLock):** [Apache License 2.0](./LICENSE)
2. **Original Rules (By Emerging Threats):** - 규칙 파일 내 명시된 SID 범위에 따라 **GPLv2, BSD, ETPRO** 라이선스가 각각 적용됩니다. 
   - 원본 규칙 배포 시 `Emerging Threats`의 저작권 문구를 반드시 유지합니다.
3. **SNORT Manual (By Cisco):** 모든 원본 권리는 Cisco에 있습니다.

---

## Reference
[http://manual-snort-org.s3-website-us-east-1.amazonaws.com/](http://manual-snort-org.s3-website-us-east-1.amazonaws.com/)