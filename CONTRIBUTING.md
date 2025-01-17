# Contribution guidelines

First off, thank you for considering contributing to db3 network

If your contribution is not straightforward, please first discuss the change you
wish to make by creating a new issue before making the change.

## Reporting issues

Before reporting an issue on the
[issue tracker](https://github.com/dbpunk-labs/db3/issues),
please check that it has not already been reported by searching for some related
keywords.

## Developing

### Build

1. clone the source and init the building environment
```shell
git clone https://github.com/dbpunk-labs/db3.git
cd db3 & bash install_env.sh
```

2. compile the metadata contract
```shell
cd  metadata && yarn && npx hardhat test
```

3. build the db3 binary

```shell
cargo build
```
4. build typescript sdk

```shell
cd sdk && make && yarn && yarn build
```

### Start Local Test Environment

```
cd tools && bash start_localnet.sh
```

### Run test cases

```
cargo test
```

