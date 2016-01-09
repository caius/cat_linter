# Cat Linter

Script to compare `cat(1)` behaviour to another binary. Test it by running against `cat`:

    $ ./cat_linter cat
    Linting cat against cat

    Checking `cat /tmp/cat_linter_file1`:
      Output matches
      Exit matches

    Checking `echo "hi\nnow" | cat`
      Output matches
      Exit matches

    Checking `cat /tmp/cat_linter_file1 /tmp/cat_linter_file2`
      Output matches
      Exit matches

    Checking `cat /tmp/cat_linter_file1 non-existent-file `
      Output matches
      Exit matches

    Checking `echo "how\nnow\nbrown\ncow" | cat /tmp/cat_linter_file1 - /tmp/cat_linter_file2`
      Output matches
      Exit matches

## License

See LICENSE.
