# DevOps Docs - Docs as Code
Project forked from [google/docsy-example](https://github.com/google/docsy-example)

## Dev enviornment

How to set your own dev enviornment?

![Containers](./assets/img/containers.png)

``` bash
 git clone --recurse-submodules --depth 1 https://github.com/facundoHernandez/devops-docs.git && cd ./devops-docs

  docker build -t devops-doc .

  docker run -p 1313:1313 -v $(pwd):/src devops-doc server

  If you want terminal detached run

  docker run -d -p 1313:1313 -v $(pwd):/src devops-doc server

```
Now you can access to check your changes http://localhost:1313