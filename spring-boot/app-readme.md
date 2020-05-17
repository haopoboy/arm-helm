## YAML template
Select an answer

### Demo
```yaml
image: 
  repository: "registry.gitlab.arm.m2m.com.tw:5000/erp4/ci-demo"
```

### SSO
```yaml
secretName: "spring"
image: 
  repository: "registry.gitlab.arm.m2m.com.tw:5000/erp3/sso-md"
ingress: 
    enabled: true
    hosts: 
      - host: "adwords.m2m.com.tw"
        paths: ["/sso"]
      - host: "dev.arm.m2m.com.tw"
        paths: ["/sso"]
```

### Search
```yaml
secretName: "search"
image: 
  repository: "registry.gitlab.arm.m2m.com.tw:5000/erp3/search-md"
ingress: 
    enabled: true
    hosts: 
      - host: "adwords.m2m.com.tw"
        paths: ["/es"]
      - host: "dev.arm.m2m.com.tw"
        paths: ["/es"]
```

### Project
```yaml
secretName: "spring"
image: 
  repository: "registry.gitlab.arm.m2m.com.tw:5000/erp3/project-md:dev"
ingress: 
    enabled: true
    hosts: 
      - host: "adwords.m2m.com.tw"
        paths: ["/"]
      - host: "dev.arm.m2m.com.tw"
        paths: ["/"]
```