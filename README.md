# sbpm
A simple bash "package" manager

```
Example usage: sbpm [ARGUMENTS] get <author/repo>
You should always use arguments before an option

Options:
    get <author/repo>    Syncs a given repository from a default host (github.com)
    clean <author/repo>  Removes a repository from cache

Arguments:
    --branch <branch>      Specifies a branch to clone
    --clone-args <args>  Specifies arguments for git clone
    --host <host>          Specifies a host from which git will clone a repo

Other:
    meow              Meow!
    help, -h, --help  Print this message
```

note: you can change the cache directory to anywhere accesible to your user in the first lines of script
