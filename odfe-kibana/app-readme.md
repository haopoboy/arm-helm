## YAML template

```yaml
es: 
  url: "https://erpes:9200"
  secretName: "odfe"
ingress: 
  enabled: true
  hosts: 
    - host: "kibana.arm.m2m.com.tw"
      paths: ["/"]
    - host: "kibana.coffee.arm.m2m.com.tw"
      paths: ["/"]
```