# Дипломная работа по DevSecOps

**Идеи:**

1. А можно ли провести атаку на цепочку поставок скомпрометировав платформу k8s? (OpenShift, DKP, RKE и другие)
2. А что если поломать сам сканер уязвимостей (заставить выдать успех при наличии уязвимостей)?
3. Компрометация сборщика (GitLab Runner, например)
4. Компрометация сервера хранилища системы контроля версий? (уяза в gitlab -> мягкое отключение сканеров)
5. Компрометация репозитория с зависимостями (nexus)?
6. Не зафиксированная в CVE/БДУ уязвимость.

**Иные материалы:**

1. [Trivy в репе Deckhouse Kubernetes Platform](https://github.com/name212/deckhouse/blob/30543731e7dfd68f49c44b4a4e4eaacabb972f4b/tools/cve/trivy-wrapper.sh)
2. [OWASP A03:2025 Software Supply Chain Failures](https://owasp.org/Top10/2025/A03_2025-Software_Supply_Chain_Failures/)
3. [OWASP Dependency Graph & SBOM Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Dependency_Graph_SBOM_Cheat_Sheet.html#example-workflows-short)
4. [OWASP Vulnerable Dependency Management Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Vulnerable_Dependency_Management_Cheat_Sheet.html#ideal-condition-of-application-of-the-approach)
5. [OWASP SSC Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Software_Supply_Chain_Security_Cheat_Sheet.html)
6. [NIST SP 800-204D](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-204D.pdf)
7. [Honeypot приложение на Java](https://github.com/cxsca/test-publicTesty)

**Статьи:**

1. https://nttdata-dach.github.io/posts/ab_softwaresupplychainsecurity_1/
2. https://habr.com/ru/articles/787190/
3. https://pvs-studio.ru/ru/pvs-studio/sca/

**Книги:**
1. Нету?

**Сканеры опен сорсные:**
1. [OWASP Dependency Check](https://github.com/dependency-check/DependencyCheck)
2. https://github.com/DependencyTrack/dependency-track
3. https://github.com/murphysecurity/murphysec
4. https://github.com/XmirrorSecurity/OpenSCA-cli

**Сканеры вражеские:**
1. Checkmarx SCA
2. Coverity
3. Fortify SCA (Micro Focus Fortify Static Code Analyzer)
4. [HCL Appscan (ранее IBM Security AppScan)](https://www.hcl-software.com/appscan/home)
5. Klocwork
6. Snyk Open Source
7. SonarQube
8. Veracode Software Composition Analysis

**Сканеры в реестре российского ПО:**
1. [CodeScoring](https://reestr.digital.gov.ru/reestr/557750/)
2. [Шерлок](https://axel.pro/sherlock)
3. [Solar appScreener](https://rt-solar.ru/products/solar_appscreener/sca/) (модуль SCA не он прем 🙂)
4. [Positive Technologies Application Inspector](https://reestr.digital.gov.ru/reestr/302603/)

**Открытые вопросы:**
1. Иные элементы SSDLC кроме SCA затрагивать или лучше сфокусироваться?

**TODO уточнить у Лёвы по анализаторам кроме trivy.**