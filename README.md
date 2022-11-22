# ClashAssets


```
rule-providers:
  ir-bank:
    behavior: "domain"    
    type: http
    url: "https://cdn.jsdelivr.net/gh/dariuosh/clashassets@main/Data/ir-bank.yaml"
    interval: 3600
    path: /ir-bank.yaml
  ir-bourse:
    behavior: "domain" 
    type: http
    url: "https://cdn.jsdelivr.net/gh/dariuosh/clashassets@main/Data/ir-bourse.yaml"
    interval: 3590
    path: /ir-bourse.yaml

rules:

  - RULE-SET,ir-bank,DIRECT
  - RULE-SET,ir-bourse,DIRECT
  - GEOIP,IR,DIRECT
```

***==> premium core only!!!***
 
