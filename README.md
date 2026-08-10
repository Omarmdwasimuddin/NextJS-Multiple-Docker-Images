# NextJS: Multiple Docker Images

## ধাপ ১: পুরনো Docker images remove করা

Old docker images remove করুন:

```bash
docker system prune -a
```

---

## ধাপ ২: প্রথম Image build করা

Image build করুন:

```bash
docker build -t nextjs-project-dockerize .
```

Docker images check করুন:

```bash
docker images
```

Container run করুন:

```bash
docker run -p 3000:3000 nextjs-project-dockerize
```

---

## ধাপ ৩: Code update করে নতুন Version build করা

Project-এর home page-এর code-এ কিছু update করুন।

তারপর নতুন version সহ image build করুন:

```bash
docker build -t nextjs-project-dockerize:12.111v .
```

নতুন version-এর container run করুন:

```bash
docker run -p 3000:3000 nextjs-project-dockerize:12.111v
```

---

## ফলাফল

এখন দুইটা Docker image-ই একসাথে browser-এ run করা যাবে।
