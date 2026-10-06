# Suricata Kuralları

SYA119 IDS/IPS dersi için başlangıç Suricata/Snort imza seti. Her kuralın neyi yakaladığı yorum satırında yazar.

## Kurallar (`rules/`)

| Dosya | İçerik |
|---|---|
| `web-saldiri.rules` | SQLi / XSS denemeleri (eşik + `msg`) |
| `tarama-tespit.rules` | Nmap SYN tarama tespiti |

## Test

```bash
suricata -T -c /etc/suricata/suricata.yaml -S rules/web-saldiri.rules
```
