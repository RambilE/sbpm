# sbpm
A simple bash "package" manager

```
sbpm - A simple bash "package" manager
Example usage: sbpm [ARGUMENTS] get <author/repo>
You should always use arguments before an option

Options:
    get <author/repo>    Syncs a given package from a default host (github) with backups of existing files
    del <author/repo>    Removes a package from store and deletes associated symlinks
    update               Updates every installed sbpm package

Arguments:
    --branch <branch>    Specifies a branch to clone
    --clone-args <args>  Specifies arguments for git clone
    --host<host>         Specifies a host from which git will clone a repo
    --nosave             Does not backup files if there is already one in specified directory
    --update-sys         Updates system packages if needed

Other:
    meow              Meow!
    help, -h, --help  Print this message
```

note: you can change the cache directory to anywhere accesible to your user in the first lines of script
