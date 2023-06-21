Summary

- Confirm repo push/pull
- A Tale of Two Maintainers
- How to cause conflicts
- How to accept an upstream change
- How to quickly update your repo
- Why use Git?


A Tale of Two Maintainers

```console
@diana
                                  HEAD
                                  |
        o---o--o-o----------o-----o
        D   M  W H          T     F

@charles
                                    HEAD
                                    |
        o---o--o-o---o--------o-----o
        D   M  W H   K        T     F

                    ^
                    |
            say what?! charles!
```

How to Resolve Conflict - Option 0 - Charles and Diana split 

```console
@diana
                                     o-----o------o   o-----o
                                    /              \ /
        o---o--o-o---o--------o-----o---o---o--o---o-o---o
        D   M  W H   K        T     F                C

@charles
```

How to Resolve Conflict - Option 1 - Charles yeets Kamila commit

```console        
@diana

                                  HEAD
                                  |
        o---o--o-o----------o-----o
        D   M  W H          T     F

@charles

        > git rebase -i (drop)

                                  HEAD
                                  |
        o---o--o-o----------o-----o
        D   M  W H          T     F
```

How to Resolve Conflict - Option 2 - Diana accepts the Kamila commit

```console        
@diana

        > git reset --hard HEAD~3
        > git pull

                                    HEAD
                                    |
        o---o--o-o---o--------o-----o
        D   M  W H   K        T     F

@charles
                                    HEAD
                                    |
        o---o--o-o---o--------o-----o
        D   M  W H   K        T     F
```

How to Clone a Repository:

    `git clone [github url]`

How to Cause a Conflict:
