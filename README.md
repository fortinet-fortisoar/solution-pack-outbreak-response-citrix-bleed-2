# Release Information 

- **Version**: 1.0.0 
- **Certified**: No 
- **Publisher**: Fortinet 
- **Compatible Version**: FortiSOAR 7.4.0 and later 

# Overview 

FortiGuard Labs has observed a sharp increase in exploitation attempts targeting the 'Citrix Bleed 2' vulnerability since July 28, 2025. Telemetry indicates activity has surged to over 6,000 detections across IPS sensors globally. The majority of observed attacks are concentrated in the United States, Australia, Germany, and the United Kingdom, with adversaries primarily focusing on high-value sectors such as technology, banking, healthcare, and education. 

 The **Outbreak Response - Citrix Bleed 2** solution pack works with the Threat Hunt rules in [Outbreak Response Framework](https://github.com/fortinet-fortisoar/solution-pack-outbreak-response-framework/blob/release/2.2.0/docs/background-information.md#threat-hunt-rules) solution pack to conduct hunts that identify and help investigate potential Indicators of Compromise (IOCs) associated with this vulnerability within operational environments of *FortiSIEM*, *FortiAnalyzer*.

 The [FortiGuard Outbreak Page](https://www.fortiguard.com/outbreak-alert/citrix-bleed-2) contains information about the outbreak alert **Outbreak Response - Citrix Bleed 2**. 

## Background: 

The vulnerability is named after the infamous Citrix Bleed Attack (CVE-2023-4966) that was previously reported around Oct 2023 and was widely exploited, by multiple threat actors, including ransomware groups. The original flaw also impacted Citrix NetScaler ADC and Gateway appliances.

CVE-2025-5777 is a critical buffer overread vulnerability dubbed as 'Citrix Bleed 2' affecting Citrix NetScaler ADC and NetScaler Gateway. The flaw stems from insufficient input validation, enabling an unauthenticated remote attacker to retrieve portions of the server’s memory. Exploiting this issue could allow attackers to access sensitive data directly from memory, potentially exposing credentials, session tokens, or other confidential information.

CVE-2025-6543 is a memory overflow vulnerability leading to unintended control flow and Denial of Service in NetScaler ADC and NetScaler Gateway when configured as Gateway (VPN virtual server, ICA Proxy, CVPN, RDP Proxy) or AAA virtual server. Citrix reports that exploitation of CVE-2025-6543 against unmitigated appliances has been observed.

CVE-2025-5349, an improper access control on the NetScaler Management Interface. 

## Announced: 

The organizations using Citrix NetScaler ADC and NetScaler Gateway appliances are strongly recommended to: Review the official Citrix security bulletins, apply all relevant patches and updates as soon as possible and monitor for any suspicious activity.

 

## Latest Developments: 

July 10, 2025: The CVE-2025-5777 vulnerability was added to CISA's Known Exploited Catalog, based on exploitation in the wild.

June 26, 2025: FortiGuard Threat Signal Report was published.
https://www.fortiguard.com/threat-signal-report/6134/citrix-netscaler-adc-and-netscaler-gateway-vulnerabilities

June 17, 2025: NetScaler ADC and NetScaler Gateway Security Bulletin published by Cirtix. 
https://support.citrix.com/support-home/kbsearch/article?articleNumber=CTX693420 

# Next Steps
 | [Installation](./docs/setup.md#installation) | [Configuration](./docs/setup.md#configuration) | [Usage](./docs/usage.md) | [Contents](./docs/contents.md) | 
 |--------------------------------------------|----------------------------------------------|------------------------|------------------------------|