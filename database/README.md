# JLU Tag Database

#### Data Source

Encyclopedia: Moegirl, Bangumi (merged);

Illustration: Pixiv.

#### Database Engine

neo4j

#### Data Format

v1:

```py
:Obj {name: ''}
:Obj:Character
:Obj:Artwork
:Obj:Label
:Obj:Label:Author
(:Artwork)<-[:_IN]-(:Character)
(:Artwork)<-[:_HAS]-(:Label)
(:Character)<-[:_HAS]-(:Label)
```

v2:

```py
:Obj {name: ''}
:Obj:Thing
:Obj:Thing:Character
:Obj:Thing:Artwork
:Obj:Label
:Obj:Label:Author
(:Artwork)<-[:_IN]-(:Character)
(:Thing)<-[:_HAS]-(:Label)
```

#### How to use

Import `neo4j.dump` to your Neo4j server.
