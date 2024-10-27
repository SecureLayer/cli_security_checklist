# CLI Security Checklist

## Objectives

Help developers making their CLI more secure. This checklist is inspired by Probely checklist and so, is supposed to be a brain exercise to ensure that essential controls are not forgotten.

Items on this list are frequently missed so it's a starting point not a bullet proof solution. Still use your brain to keep your CLI secure (please). 

## The checklist
#### SSH key management
- [ ] My SSH keys are generated with strong algorithms (e.g., RSA 4096 or Ed25519)
- [ ] My private keys are stored securely and have proper permissions
- [ ] There are no unprotected or unnecessary keys on my laptop
#### Environment variables
- [ ] I do not have any sensitive information (API keys, passwords) stored in environment variables
- [ ] Sensitive informations are not hardcoded in scripts or configuration files
#### Command history
- [ ] There is no sensitive commands (e.g., those exposing credentials or deleting data) recorded in my history
- [ ] Command history is appropriately configured to ignore sensitive command
#### Installed tools and packages
- [ ] My tools or libraries no not have known vulnerabilities (using tools like `npm audit` for Node.js)
- [ ] My package manager is configured to update dependencies regularly
- [ ] I regularly check installed packages and delete unused ones  
#### Access control and permissions
- [ ] My sensitive files (like private keys or configuration files) have restrictive permissions
- [ ] I am using the least privilege principle for accessing systems and resources
#### Exposure of sensitive information
- [ ] No configuration files or scripts have been (inadvertently!) shared in version control (e.g., `.gitignore` settings)
- [ ] Logs do not expose sensitive information
#### Security updates and patching
- [ ] My critical software and tools are up to date (e.g., `npm update` or `yarn update`)
- [ ] I updated my package manager less than 48h ago

If you need help checking these boxes ping me!


version 0.1
