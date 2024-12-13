# Get the current user's username (from the home directory)
$CurrentUsername = $env:USERNAME

# Define the path to the JSON file, including the current user's directory
$SearchFile = "C:\Users\$CurrentUsername\AppData\Roaming\something\File.json"  # Update as needed

# Define the string to search for and replace
$SearchString = "YourSearchString"  # Update with the text you want to search for

# Check if the file exists
if (-not (Test-Path -Path $SearchFile)) {
    Write-Host "Error: File not found at $SearchFile"
    exit 1
}

# Read the file content as text
try {
    $FileContent = Get-Content -Path $SearchFile -Raw
} catch {
    Write-Host "Error: Unable to read the file."
    exit 1
}

# Perform the search and replace
if ($FileContent -match [regex]::Escape($SearchString)) {
    $UpdatedContent = $FileContent -replace [regex]::Escape($SearchString), $CurrentUsername
    Write-Host "Replaced occurrences of '$SearchString' with '$CurrentUsername'."
} else {
    Write-Host "Error: String '$SearchString' not found in the file."
    exit 1
}

# Save the updated content back to the file
try {
    Set-Content -Path $SearchFile -Value $UpdatedContent
    Write-Host "File updated successfully."
} catch {
    Write-Host "Error: Unable to save changes to the file."
    exit 1
}