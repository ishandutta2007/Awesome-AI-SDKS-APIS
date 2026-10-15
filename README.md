# Awesome-AI-SDKS-APIS

$ErrorActionPreference = "Continue"
$repo_name = if ([string]::IsNullOrEmpty($repo_name)) { (Get-Item .).Name } else { $repo_name }
$real_repo_name = $repo_name -replace '^Awesome-',''
$owner = "ishandutta2007"

git add README.md; git commit -m "first code" 2>$null
git pull --no-edit 2>$null; git push 2>$null

if (Test-Path "..\Awesome-BERT\.gitignore") {
    cp ..\Awesome-BERT\.gitignore .; git add .gitignore; git commit -m "add .gitignore" 2>$null
}
if (Test-Path "..\Awesome-BERT\LICENSE") {
    cp ..\Awesome-BERT\LICENSE .; git add LICENSE; git commit -m "add LICENSE" 2>$null
}
$bak = git ls-files "*.bak"
if ($bak) { git rm --cached *.bak }

git add .; git commit -m "cleanup" 2>$null; git push

gh repo edit "$owner/$repo_name" --add-topic "curated-list,awesome-list,opensource"

# Regenerate README (uncomment when ready):
# $loops_path = "C:\path\to\loops"
# chatgpt-cli "$loops_path\sheet_outputs\$real_repo_name.txt" -o "../$repo_name/README.md" -w 600
# grok-cli "$loops_path\sheet_outputs\$real_repo_name.txt" -o "../$repo_name/README.md" -w 600
