# HomeLab Cloud Init Bootstrapping
## Building
To build the user-data and meta-data files, which will be placed in the ./dist
folder, execute:
```sh
pnpm build
```

## Cloud-init Bootstrapping
Add the following kernel parameters to a cloud-init enabled boot disc:
```
ds=nocloud-net;s=https://scraswell.github.io/pub-bootstrapping/cloud-init/dist/debian/
```