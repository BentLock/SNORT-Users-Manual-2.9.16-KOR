# 🛡️ SNORT 2.9.16 가이드 (KOR)

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![SNORT Version](https://img.shields.io/badge/SNORT-2.9.16-red.svg)](http://manual-snort-org.s3-website-us-east-1.amazonaws.com/)
[![Author](https://img.shields.io/badge/Author-BentLock-orange.svg)](https://github.com/BentLock)

> **SNORT 2.9.16 공식 매뉴얼 기반 한국어 Rule 가이드입니다.**
>
> *\* 작성자는 전문 번역가가 아닙니다. 작성자의 주관적 해석이 포함되어 있으나, 원문의 의도를 가급적 훼손하지 않도록 노력하고 있습니다.*
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
		- [3.4.1 msg](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#341-msg)
		- [3.4.2 reference](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#342-reference)
		- [3.4.3 gid](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#343-gid)
		- [3.4.4 sid](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#344-sid)
		- [3.4.5 rev](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#345-rev)
		- [3.4.6 classtype](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#346-classtype)
		- [3.4.7 Priority](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#347-priority)
		- [3.4.8 metadata](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#348-metadata)
		- [3.4.9 General Rule Quick Reference](./3.-Writing_Snort_Rules/3.4-General_Rule_Options.md#349-general-rule-quick-reference)


---

## 📜 라이선스 및 저작권 안내 (License & Copyright)

* **Author:** BentLock (Individual Contributor)
* **원저작권 (Original Work):** SNORT 및 관련 로고, 공식 매뉴얼 원본의 저작권은 **Cisco and/or its affiliates**에 있습니다.
* **오픈소스 라이선스:** 이 저장소의 한국어 요약 및 분석 내용은 [Apache License 2.0](./LICENSE)에 따라 배포됩니다. 
    * 개인의 학습 및 실무 참고용으로 자유롭게 활용 가능하며, 재배포 시 출처(BentLock)를 명시해 주세요.

---

## Reference
- [http://manual-snort-org.s3-website-us-east-1.amazonaws.com/](http://manual-snort-org.s3-website-us-east-1.amazonaws.com)

- [도서 : 네트워크_보안전문가로_가는_길](https://product.kyobobook.co.kr/detail/S000001732466)