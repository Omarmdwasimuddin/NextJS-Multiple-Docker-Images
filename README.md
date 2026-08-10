## NextJS: Multiple Docker Images

#### Old docker images remove koro
```bash
docker system prune -a
```
---

#### images build koro
```bash
docker build -t nextjs-project-dockerize .
```
---

#### check docker images
```bash
docker images
```
---

#### docker containters run 
```bash
docker run -p 3000:3000 nextjs-project-dockerize
```
---

#### project home page er code e kichu update koro
> new docker images build koro version add kore.
```bash
docker build -t nextjs-project-dockerize:12.111v .
```
---


#### ekhon duita docker images kei brower e ekshathe run kora jabe.
