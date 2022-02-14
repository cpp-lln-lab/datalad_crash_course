<h1 style="width: 120%"> Datalad crash course </h1>

<!-- insert datalad and crash test dummies image -->

<h2 id="TOC"> Table of content </h2>

- [Goals](#goals)
- [Prerequisites](#prerequisites)
    - [Pre-flight checks](#pre-flight-checks)

<details><summary> <b>CLICK ME</b> </summary><br>

... to see what I hide !!!

</details>

<br>

## Goals

- be able to install a datalad dataset and work with it
- be able to create a datalad dataset and a remote copy of it online

## Prerequisites

In terms of technical knowledge, knowing some UNIX command line and some of the
Git basics might help but are not required.

But there are things you need to install and do before the workshop:

- [install datalad](http://handbook.datalad.org/en/latest/intro/installation.html)
- [create a GIN account](https://gin.g-node.org/)
- [create an SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
- add it to your GIN account:
  - [help see the github doc](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
  - [help in the datalad handbook](http://handbook.datalad.org/en/latest/basics/101-139-gin.html#prerequisites)
- [basic configuration](http://handbook.datalad.org/en/latest/intro/installation.html#initial-configuration)

### Pre-flight checks

Checks to make sure everything is set up correctly

In a terminal, make sure that you have a version of datalad >= 0.13

```bash
datalad --version
```

```bash
datalad 0.13.4
```

Try to install a dataset from GIN

```bash
datalad install -s git@gin.g-node.org:/cpp-lln-lab/CPP_visMotion-raw.git \
                  ~/CPP_visMotion-raw
```

```bash
install(ok): /home/remi/CPP_visMotion-raw (dataset)
```

The first time you do this, it will ask you some confirmation about using your
SSH key to connect to GIN. This is normal and you can safely say "yes".

If this install work you can remove the dataset with.

```bash
rm -rf ~/CPP_visMotion-raw
```
