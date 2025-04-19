## Finding .yml files in current directory and subdirectories

`find . -name "*.yml"`

* Searches current directory (.) for files ending in .yml
* Find searches recursively by default

## Find .yml files that contain substring `vector` in current directory and subdirectories

find . -name "*.yml" -exec grep -l "vector" {} \;

* -l option in grep only returns the NAMES of files that match
* By default, grep returns the matching lines
