# Hello World

## Deployment

### Setup

#### Database

Dev / test:

- Replica set: `dev001`
- Database: `helloworld`

Production:

- Replica set: `prod001`
- Database: `helloworld`

Create tables:

```
/usr/local/bin/mysql_utils/mysql_cli.py -p read-write <replica set>
source ~/code/hello-world/db/ddl.sql
```

### Build

```
make build_all
```

### Run

```
make run_hw
```

## Useful info

- [README](https://github.com/ggdamn/hello-world)
