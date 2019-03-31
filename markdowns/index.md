# About

This is for myself 3 days from now.

```plantuml
@startuml
scale 700 width

interface DevOps{
    Reduce organization silos()
    Accept failure as normal()
    Implement gradual change()
    Leverage tooling & automation()
    Measure everything()
}

class SRE{
    Share Ownership()
    Error Budget()
    Canary Release()
    Automate common case()
    Measure Toil and Reliability()
}
Class SE{
    Monitor Systems()
    Improve Performance()
    Design Systems()
}
Class Contributor{
    OSS
    Review Code()
    Raise Issue()
    Fix Issue()
    Fix Docs()
    Create Feature()
}

class SRETeam{
    SLO
    SLI
    availability()
    latency()
    performance()
    efficiency()
    change management()
    monitoring()
    emergency response()
    capacity planning()
}

object Me
Me : Name = Wang Shuang
Me : Age = 32+
Me : Role = Tech Lead
Me : OSS = [Ansible, Docker]


DevOps <|-- SRE
SRETeam o-- SRE : aggregation

Me --|> Contributor
Me --|> SRE
Me --|> SE

@enduml
```
