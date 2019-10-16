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

## Technologies

The core part of the application is a .NET-application (WPF) written in VB.NET. 
The whole communication with CATIA is done through the CATIA Automation-API. Therefore another part of the application is written as macros in VBA.

Data is stored in an Access database to enable easy manipulation of certain datasets from a wide range of people.

## User Interface


## Algorithms

