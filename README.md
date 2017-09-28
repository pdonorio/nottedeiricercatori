
# La notte dei ricercatori

Sperimentiamo grazie a Python e i "Notebook" cosa vuol dire
essere nei panni di un ricercatore scientifico per un giorno!

---

## Istruzioni per replicare l'ambiente di lavoro

1. Installare [docker](https://www.docker.com/community-edition)
2. Lanciare il seguente comando da terminale:

```bash
# Avviare un container con jupyter 
# e il materiale scaricato da GitHub

docker run \
    -e LECTURE_REPO: github.com/pdonorio \
    -e LECTURE_PRJ: nottedeiricercatori \
    -e LECTURE_BRANCH: master \
    -e LECTURE_PATH: ROMA \
    -d --name ndr -w /tmp -v mydata:/tmp -p 80:8888 \
    cineca/allspark:rise
```


