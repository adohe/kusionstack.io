# prometheus

## Schema Prometheus

Prometheus can be used to define monitoring requirements

### Attributes

| name | type | description | default value |
| --- | --- | --- | --- |
|**path**|str|The path to scrape metrics from.|"/metrics"|
|**port**|str|The port to scrape metrics from. When using Prometheus operator, this needs to be the port NAME. Otherwise, this can be a port name or a number.|container ports when scraping pod (monitorType is pod) and service port when scraping service (monitorType is service)|

### Examples
```python
import monitoring as m

"monitoring": m.Prometheus {
    path:           "/metrics"
    port:           "web"
}
```

<!-- Auto generated by kcl-doc tool, please do not edit. -->
