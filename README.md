# graylog-grok-patterns
GROK patterns for use with Graylog 2.x as Input Extractors

## Contents
1. `cisco-asa.json` - an extractor for all Deny type Syslog messages from Cisco ASA v9.5 (any maybe others)
2. `cisco-firepower.json` - an extractor for SFIMS Syslog messages from ASA Firepower Modules v6.1 (and maybe others)
3. `trendmicro-deepscan-cef.json` - an extractor for CEF Syslog messages from TrendMicro DeepScan v9.x (and maybe others)
3. `iis-w3c-extended.json` - an extractor for web log files in IIS W3C Extended (6.x+) format (and maybe others)

## Prerequisites

The Cisco patterns require the following `System` / `Grok Patterns` be installed on your Graylog server:
```
CISCOTIMESTAMP
%{MONTH} +%{MONTHDAY}(?: %{YEAR})? %{TIME}
```
