# Learn the Commandline

Scripts and resources to learn the command line.

If using these to learn the command line,
start with the ``learn-the-cli`` script
and then follow with ``learn-the-filesystem``.

The ``learn-the-cli-module`` allows users to
select specific modules to study.

The ``flashcards`` script is for
memorizing some of the commands covered in the
other two scripts,
plus some others.

## To Download

If your ``~/bin`` directory is in your ``$PATH``
(check with ``echo $PATH`` at your command prompt),
then you can download the scripts there.
If ``~/bin`` is not in your ``$PATH``, and
you don't know how to add it,
then you can download the scripts to the
``/usr/local/bin`` directory:

### ``/usr/local/bin`` instructions

If ``~/bin`` is not in your ``$PATH``, or if you want the
scripts available to all users on a single system, then
follow these instructions:

```
git clone https://github.com/cseanburns/learn-the-commandline.git
sudo cp learn-the-commandline/* /usr/local/bin
```

### ``~/bin`` instructions

To add ``~/bin`` to your ``$PATH``, add the following
to your **~/.bashrc** file using your preferred text editor:

```
PATH="$HOME/bin${PATH:+:${PATH}}"; export PATH;
```

Create the directory if it does not yet exist:

```
mkdir ~/bin
```

Then run the following commands:

```
git clone https://github.com/cseanburns/learn-the-commandline.git
cp learn-the-commandline/* ~/bin
```

### Learn the Commandline

To run the programs, type the name of the script.

## TODO

- Need to check that file and directory names used in the
  ``learn-the-*`` scripts do not already exist before running
  the scripts.
- Add the cards.csv data to the ``flashcards`` script to
  keep it to one file.
- Modularize the ``learn-the-filesystem`` script
