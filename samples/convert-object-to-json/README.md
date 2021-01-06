# Convert object type parameter to JSON string
convertToJson function can convert object to JSON string.

## How to run
1. Create a Azure pipeline and select "Existing Azure Pipelines YAML file".
1. Set path as "/samples/convert-object-to-json/ci.yml".
1. Run manually.
1. You can download a JSON file as an artifact.

## Output
- PowerShell task
```
Starting: PowerShell
==============================================================================
Task         : PowerShell
Description  : Run a PowerShell script on Linux, macOS, or Windows
Version      : 2.179.1
Author       : Microsoft Corporation
Help         : https://docs.microsoft.com/azure/devops/pipelines/tasks/utility/powershell
==============================================================================
Generating script.
========================== Starting Command Output ===========================
"C:\windows\System32\WindowsPowerShell\v1.0\powershell.exe" -NoLogo -NoProfile -NonInteractive -ExecutionPolicy Unrestricted -Command ". 'D:\a\_temp\a9567c9c-2558-486b-95fb-b6a839dfa6b5.ps1'"
{
  "name": "Alice",
  "country": "Japan",
  "prefecture": "Tokyo",
  "friends": [
    "Bob",
    "Carol",
    "Dave"
  ]
}
My name is @{name=Alice; country=Japan; prefecture=Tokyo; friends=System.Object[]}.name
I live in Tokyo, Japan.
These are my friends
Bob
Carol
Dave
Finishing: PowerShell
```

# Blog post about this
[Azure Pipelines で object 型のパラメーターを JSON に変換する](https://qiita.com/t104/items/b81d87e9e54db7a7e4e1)
