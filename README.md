# App-development
Creating this repo for my mobile app development


# Store results in variables
$psVersion = $PSVersionTable.PSVersion
$currentDir = Get-Location
$folderList = Get-ChildItem -Recurse -Directory  # List only directories recursively

# Print the stored variables with descriptions
Write-Host "PowerShell Version: $psVersion"
Write-Host "Current Working Directory: $currentDir"
Write-Host "List of Directories Recursively:"

# Print the folder list
$folderList | ForEach-Object { Write-Host $_.FullName }