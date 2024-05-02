trigger:
- main
 
pool:
  vmImage: 'ubuntu-latest'
 
steps:
- task: PythonScript@0
  inputs:
    scriptSource: 'inline'
    script: |
      print("Hello World")
  displayName: 'Run Hello World Script'
