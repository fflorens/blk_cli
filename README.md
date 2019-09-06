# blk_cli

A quick and dirty cli for scw block storage in python3

## Depencies :
requests

## Using :

Size for volume is in gb, subcommands are `create`, `delete`, `list`, `attach` and `detach`.
```
usage:
blk_cli <-t|--token> <token> <-o|--organization> <organization> <command> [<args>]

Avaible commands:
 create         Create a block volume
 delete         Delete a block volume
 attach         Attach a block volume to a server
 detach         Detach a block volume from a server
 list           List block volumes

See 'blk_cli <command> help' for further information.
```

For example :

```
$> ./blk_cli -t $SCW_TOKEN -o $SCW_ORGANIZATION create --name block101 --size 10
ce009fa9-3876-4ba8-a494-e230bd35817c
```
