# _DockerStation_
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/dvstLab/DockerStation/builder?style=for-the-badge)
![GitHub](https://img.shields.io/github/license/dvstLab/DockerStation?style=for-the-badge)
  
## WHat is this?
  A collection of some dockerfiles to simplify deployments.
  
## Usage/Examples

### Userge

Change your Dockerfile, example:

```bash
FROM rzlamrr/userge:latest

COPY . .

CMD bash run
```

### Slam-mirrorbot

Change your Dockerfile, example:

```bash
FROM rzlamrr/megasdk:latest

COPY . .
COPY .netrc /root/.netrc

RUN chmod +x aria.sh

CMD ["bash","start.sh"]
```

### DaisyXmusic

Change your Dockerfile, example:

```bash
FROM rzlamrr/music:latest

COPY . .

CMD ["python3", "-m", "DaisyXMusic"]
```

## FAQ

#### Can i use this for other repo?

You can use it to other repo that similiar.

#### Deployment failed, what should i do?

Just open issue, or do a PR. Contributions are always welcome!

## License

[GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)
