# Policy As Code - WB3Tech Microgrid

Contains all the policy, compliance, and security as code for all WB3Tech Microgrid systems.  All repositories with a policy-as-code are intended to run in a production environment.

## Repository Structure

This repo is primarily structrued as a monorepo.  It is strucutre as follows.

- The first level of a directories are either a WB3Tech Microgrid project, or the name of an upstream project.
  - This name is a logical grouping and not specifically related to any repostiories within WB3Tech Microgrid
- Within a first-level directory, you'll find directories named according to the repository within th WB3Tech Microgrid organization.
  - These second-level directories contain all the policy as code for the SDLC of the technology within that repository.

**Policy As Code - Structure Model**

```
.
+-- README.md
+-- [WB3Tech Microgrid Project Name]
|   +-- [WB3Tech Microgrid repository name]
|       +-- policy-as-code.file
|       +-- [policy-as-code subdirectory]
|          +-- policy-as-code.file
+-- [Upstream Project Name]
|   +-- [Forked Upstream repository name]

```

**Policy As Code - Example**

- Hyphae is an upstream Linux Foundation Energery (LFEnergy) project.
  - Each subdirectory of this directory is the name of the corresponding WB3Tech Microgrid repository name.

```
.
+-- README.md
+-- Hyphae
|   +-- hyphae-apis
|   +-- hyphae-apis-containers
|   +-- etc...
+-- 
|   +-- [WB3Tech Microgrid repository name]

```