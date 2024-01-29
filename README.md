# CGMES Profiles

## Generating the Documentation
1. Have the virtual environment active which has the dependencies in `pyproject.toml` satisfied.
2. Delete all Markdown files in all the profile subdirectories of `_docs`. Make sure to not touch the `assets` subdirectory, i.e. for each profile subdirectory run something like:
```shell
$ rm _docs/'PROFILE_DIR'/*.md
```
3. Generate the static Markdown files for each profile.
```shell
$ gen-doc -d _docs/'PROFILE_DIR' --diagram-type mermaid_class_diagram --template-directory _templates/ --use-slot-uris /path/to/your_schema.yaml
```
4. Delete slot and type pages, since these cause problems and don't provide us anything meaningful for the CGMES profiles. A handy way of doing this is to navigate to the profile directory and then run:
```shell
$ grep -E '^# (Slot|Type): ' *.md -l | xargs rm
```
5. Generate the static HTML website:
```shell
$ mkdocs build
```
6. The index pages of the profiles have some references to LinkML types that we need to remove manually. Running `mkdocs build` again tells you what the dead references are. Remove these entries from the classes table in `index.md` and build again.
