![By ULHPC](https://img.shields.io/badge/by-ULHPC-blue.svg) [![github](https://img.shields.io/badge/git-github-lightgray.svg)](https://github.com/ULHPC/demonstrators) [![Issues](https://img.shields.io/badge/issues-github-green.svg)](https://github.com/ULHPC/demonstrators/issues)

                 _   _       _   _         _   _ ____   ____
                 | | | |_ __ (_) | |_   _  | | | |  _ \ / ___|
                 | | | | '_ \| | | | | | | | |_| | |_) | |
                 | |_| | | | | |_| | |_| | |  _  |  __/| |___
                  \___/|_| |_|_(_)_|\__,_| |_| |_|_|    \____|

        ____                                 _             _
       |  _ \  ___ _ __ ___   ___  _ __  ___| |_ _ __ __ _| |_ ___  _ __
       | | | |/ _ \ '_ ` _ \ / _ \| '_ \/ __| __| '__/ _` | __/ _ \| '__|
       | |_| |  __/ | | | | | (_) | | | \__ \ |_| | | (_| | || (_) | |
       |____/ \___|_| |_| |_|\___/|_| |_|___/\__|_|  \__,_|\__\___/|_|
                                                                                                                                
                                                                                                                                
       Copyright (c) 2020 UL HPC Team <hpc-team@uni.lu>

[UL] HPC demonstrator for applications run on the UL HPC facility and its partners

## Installation / Repository Setup

This repository is hosted on [Github](https://github.com/ULHPC/demonstrators).

* To clone this repository, proceed as follows (adapt accordingly):

```bash
$> mkdir -p ~/git/github.com/ULHPC/
$> cd ~/git/github.com/ULHPC/
$> git clone git@github.com:ULHPC/demonstrators.git
```


**`/!\ IMPORTANT`**: Once cloned, initiate your local copy of the repository by running:

```bash
$> cd demonstrators
$> make setup
```

This will initiate the [Git submodules of this repository](.gitmodules) and setup the [git flow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow) layout for this repository. Later on, you can update your local branches by running:

     $> make up

If upon pulling the repository, you end in a state where another collaborator have upgraded the Git submodules for this repository, you'll end in a dirty state (as reported by modifications within the `.submodules/` directory). In that case, just after the pull, you **have to run** `make up` to ensure consistency with regards the Git submodules:

Finally, you can upgrade the [Git submodules](.gitmodules) to the latest version by running:

    $> make upgrade

## Issues / Feature request

You can submit bug / issues / feature request using the [`ULHPC/demonstrators` Project Tracker](https://github.com/ULHPC/demonstrators/issues)

## Contributing

That's quite simple:

1. [Fork](https://help.github.com/articles/fork-a-repo/) it
2. Create your own feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new [Pull Request](https://help.github.com/articles/using-pull-requests/)
