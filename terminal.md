# Terminal

As a UNIX OS base user I :love: terminal, and I am here to share some ninjutsu that I use.

## MPlayerX Playlist

I have a Mac and like must of you I use MPlayerX to view videos, and like must of you I miss the play list feature
when I am seeing my weekly shows. So with the help of my trusty terminal I created a turn around.

```bash
i=9900; for file in *; do mv "$file" "$i-$file"; ((i = i +1)); done;
```

This script prefixes every file with a sequencial number, and when played at the MPlayerX, he will
play the files by the order of the prefix.

For easy access you can always create an alias for the inline script.