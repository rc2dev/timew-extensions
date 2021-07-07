# timew-extensions

This repository holds the Timewarrior extensions I use.

## Extensions

- My modified version of `totals.py`, with these changes:

	|                   | My version                                           | Original                                              |
	|-------------------|------------------------------------------------------|-------------------------------------------------------|
	| Sort tags         | By total time, descending.                           | Alphabetically.                                       |
	| Total time        | Real, clock time, like `timew summary`.              | The sum of every tag. A period with multiple tags will be sumed multiple times. |
	| Productive time   | Also print the total time spent on productive tags.  | -                                                     |
	| Unproductive tags | Show a marker on unproductive tags.                  | -                                                     |

	To use the productive related features, set `custom.unproductive_tags` on Timewarrior config. For example, to set foo and bar as unproductive:

	```sh
	timew config custom.unproductive_tags foo,bar
	```

## License

Please refer to the header of the extension file.

