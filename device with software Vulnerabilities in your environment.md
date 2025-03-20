DeviceTvmSoftwareVulnerabilities
| where CveId in ("CVE-****-****") //add the CVE number in CVE-****-****
| summarize dcount(DeviceId) by OSPlatform, SoftwareVendor, SoftwareName, SoftwareVersion
