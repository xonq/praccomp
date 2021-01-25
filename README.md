# Repository for assignment 1
## files within repository
- newfile.md
	- an explanation of how to start, maintain, and why to use sourdough
- creating data
	- used the following `for` command (which corrected for me not initially using `git mv`):

```bash
for name in $(find data); do name1=$(basename $name ".csv").txt; newname=$(basename $name1 ".txt").csv; git mv $name1 data/$newname; done
```
