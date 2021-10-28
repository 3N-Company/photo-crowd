# Photo Crowd

This application was developed for Open Data Camp 2021.
Photo Crowd is aimed to use the power of the crow to annotate unknown odl images.

## Deploy

You need to create two empty folders (`colorised` & `upscaled`) inside the 
`photo` folder.

```bash
mkdir -p ./photo/colorised ./photo/upscaled
```

> Note: Upscale will work only if you put upscaled photos in the 
> `/photo/upscaled` folder.

Then just simply start docker:

```bash
docker-compose up
```

Then simply open the [localhost](http://localhost).

## Architecture

This repository uses the composition of several services as show below.

![Current Architecture](.github/public/architecture.png)

You can found these repositories under:
- Frontend - [3N/pc-frontend](https://github.com/3N-Company/pc-frontend)
- Core - [3N/pc-core](https://github.com/3N-Company/pc-core)
- Normalisation - [3N/pc-normalisation](https://github.com/3N-Company/normalisation)
- Colorisation - [3N/pc-colorisation](https://github.com/3N-Company/colorisation)
