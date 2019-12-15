# Opencast Workflow Turing Machine

This repository demonstrates one way to use Opencast's workflow system to implement a turing machine.

Use `docker-compose` to run a standard Opencast Docker image:

```sh
$ docker-compose up
```

To create the workflows that implement a particular turing machine, use the `turing` script:

```sh
$ ./turing
```

You can edit the header of the file to implement your own turing machines. Rerunning the script will generate all files
anew.

`turing` also generates scripts for each given example input to ingest the necessary files and start the Opencast
workflow, i.e. the turing machine:

```sh
$ ./bin/wikipedia-example1.sh
```

To delete all existing files, you can use the `turing-clean` script.
