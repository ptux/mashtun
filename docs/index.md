# About me

```plantuml
@startuml
scale 800 width
scale 700 height

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

Class BackEndEngineer{
    Monitor Systems()
    Improve Performance()
    Design Systems()
}

Class FrontEndEngineer{
    Monitor Systems()
    Improve Performance()
    Design Systems()
}

Class InfraEngineer{
    Monitor Systems()
    Improve Performance()
    Design Systems()
}

Class Contributor{
    OSS = [ Ansible, Docker,Kubernetes ]
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
Me : Age = 1985
Me : Role = Tech Lead
Me : Tobe = Product manager


DevOps <|-- SRE
SRETeam o-- SRE

Me --|> Contributor
Me --|> SRE
Me --|> InfraEngineer

@enduml
```
