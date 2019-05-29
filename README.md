# contrail_backup
Contrail backup playbook for RHOSP13

## Description

This repository is Contrail backup and restore tool of ansible base.
Implementation is referring to the following URL.

[Backing Up Contrail Databases Using JSON Format](https://www.juniper.net/documentation/en_US/contrail5.1/topics/concept/backup-using-json-40.html)


## How to use this tool

This tool target to RHOSP13 and Contrail 5.x environment.

***Very easy in 3 steps !!!***

Other requirements are listed below:

- ansible: 2.4.6.0 or later
- Execute this tool on director node

To work on the contrail_backup, clone this repository on the director node:
```
git clone https://github.com/JuniperJapan/contrail_backup
```

### 1. Create inventory file

```
cd contrail_backup
./create_inventory.sh
```

### 2. Cassandra database dump and Cassandra's directory,Zookeeper directory backup.

```
./backup.sh
```

### 3. Restore cassandra.

```
./restore.sh
```

:)

## Licence

[MIT](https://github.com/tcnksm/tool/blob/master/LICENCE)

## Author

[konono](https://github.com/konono)

