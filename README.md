# DataPipeline
CAS data preparation tool to automatically optimize CAS data from CATIA for visualization in systems like Unity. Project was done as part of my diploma thesis with BMW.

Includes four stages: 
- Data preparation
  (Joining surface patches, analyzing resulting joined surfaces [bounding box, triangle counts, etc.],
  naming conventions, ...)
- Structure management
  (Changing the flat structure into PDM-friendly structure, adding transformations, etc.)
- Tesselation
  (Algorithm categorizes joined surfaces in order to create an optimally tesselated model, 
    algorithm to figure out the right sag value)
- Quality asessement

[Graphic]

The core part of the application is a .NET-application (WPF) written in VB.NET. 
The whole communication with CATIA is done through the CATIA Automation-API. Therefore another part of the application is written as macros in VBA.

Data is stored in an Access database to enable easy manipulation of certain datasets from a wide range of people.

## User Interface

![alt text](https://raw.githubusercontent.com/maxvoi/DataPipeline/master/Img/UI.png)

## What I learned

#### Languages
Deepened my understanding of the .NET (C# and VB.NET)-world\
Experimented with C++ (within the Architecture of CATIA)

#### Design Patterns
WPF is based on the MVVM pattern, which created a nice opporturnity to deeply understand the MVVM pattern.

#### Datastrucutures & Algorithms
Writing own algorithms (Divide & Conquer, ...) and understanding a lot of tesselation and simplification algorithms I learned a lot about algorithm design.

Writing an application, which at it's core is a tool to convert one complex data structure into another similar data structure (with key differences), I learned a lot about graphs and trees. 

#### Database
Avoiding external dependencies as much as possible I wrote my own little library for accessing the database with SQL-queries.

#### Software
Gained a lot of insights into Unity\
CATIA (APIs, general structure and architecture)
