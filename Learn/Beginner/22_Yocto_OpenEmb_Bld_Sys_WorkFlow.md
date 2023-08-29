## Yocto/Open Embedded BuildSystem Workflow

- Developers specify architecture, policies, patches and configuration details

- The build system fetches and downloads the source code from the specified location supports downloading torballs and source code repository system such as git

- Extracts the source into a local workspace area

- Patches are applied 

- Configuring and compiling the software and run
Installs te software into a temp staging area depending on the user configuration, deb/rpm/ipk binaries are generated

- The build system generates a binary package feed that is used to create the final root file image

- Finally generates the file system image and a customized extensible SDK for application development in a parallel
