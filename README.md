# Security-Guardian
![Guardian Security Status](https://github.com/Moises-its/Security-Guardian/actions/workflows/guardian-security.yml/badge.svg)
 
### THIS FILE IS NOT "PLUG AND PLAY" ###

**Yaml file calls for 3 seperate tokens and without them the Guardian will not have permission to scan

1. GitGuardian API is required through free account
2. SNYK Token is required through free account
3. CodeQL is built into GitHub but ensure "GitHub Advanced Security" is enabled in settings

**Linter Requirment

The line "run: npm run lint" assumes website has a lint script defined in their "package.json"

For this ensure package.json has the following in their package.json file:

"scripts": {
  "lint": "eslint, --ext .js,.jsx,.ts,.tsx"
  }

**Layer 5 - Docker Requirment

if said project is just a folder of React files then Dockerfile will fail

if Docker is not being used, commit out

**CodeQL Languages

Current YAML file is set to scan for javascript, python and typescript

If repo contains different languages the file will get confused and ignore it
